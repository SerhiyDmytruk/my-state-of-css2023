## [Anchor positioning](https://developer.chrome.com/blog/whats-new-css-ui-2023/#anchor-positioning)

[w3c](https://www.w3.org/TR/css-anchor-position-1/) spec
[kizu](https://kizu.dev/anchor-positioning-experiments/) simple words

#### [Browser support](https://developer.chrome.com/blog/tether-elements-to-each-other-with-css-anchor-positioning/#browser-support)

You can try out the CSS anchor positioning API in Chrome Canary behind the "Experimental Web Platform Features" flag. To enable that flag, open Chrome Canary and visit chrome://flags. Then enable the "Experimental web platform features" flag.

There is also a polyfill in development by the team at Oddbird. Be sure to check the repo at github.com/oddbird/css-anchor-positioning.

You can check for anchoring support with:

@supports(anchor-name: --foo) {
  /* Styles... */
}
Note that this API is still in an experimental stage and could change. This article covers the important parts at a high level. The current implementation also isn't completely in sync with the CSS Working Group spec.

#### The main idea
Popovers are also frequently used in elements such as dialogs and tooltips, which typically need to be anchored to specific elements. Take this event example. When you click on a calendar event, a dialog appears near the event you’ve clicked on. The calendar item is the anchor, and the popover is the dialog which shows the event details.

You can create a centered tooltip with the anchor() function, using the width from the anchor to position the tooltip at 50% of the anchor’s x position. Then, use existing positioning values to apply the rest of the placement styles.

But what happens if the popover doesn’t fit in the viewport based on the way you’ve positioned it?


[![Issue when we try make positioning](https://wd.imgix.net/image/HodOHWjMnbNw56hvNASHWSgZyAf2/wlIsaOjCC0lVKzMp2fCF.png?auto=format&w=845)](https://developer.chrome.com/blog/whats-new-css-ui-2023/#anchor-positioning)


To solve for this, the anchor positioning API includes fallback positions that you can customize. The following example creates a fallback position called "top-then-bottom". The browser will first try to position the tooltip at the top, and if that doesn’t fit in the viewport, the browser would then position it under the anchoring element, on the bottom.

```
.center-tooltip {
  position-fallback: --top-then-bottom;
  translate: -50% 0;
}

@position-fallback --top-then-bottom {
  @try {
    bottom: calc(anchor(top) + 0.5rem);
    left: anchor(center);
  }

  @try {
    top: calc(anchor(bottom) + 0.5rem);
    left: anchor(center);
  }
}
```

https://storage.googleapis.com/web-dev-uploads/video/Dyx9FwYgMyNqy1kMGx8Orz6q0qC3/X79WdPJ5bZDXhJ3Fw7Ti.mp4