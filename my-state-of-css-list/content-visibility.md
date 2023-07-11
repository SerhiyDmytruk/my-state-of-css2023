## [content-visibility](https://developer.mozilla.org/en-US/docs/Web/CSS/content-visibility)

> The `content-visibility` CSS property controls whether or not an element renders its contents at all, along with forcing a strong set of containments, allowing user agents to potentially omit large swathes of layout and rendering work until it becomes needed. It enables the user agent to skip an element's rendering work (including layout and painting) until it is needed — which makes the initial page load much faster.

> `content-visibility` relies on primitives [within the the CSS Containment Spec](https://drafts.csswg.org/css-contain/). While content-visibility is only supported in Chromium 85 for now (and deemed "worth prototyping" for Firefox), the Containment Spec is supported in [most modern browsers](https://caniuse.com/css-containment).

____

> The solution to big layout shifts is to pair `content-visibility: auto;` with `contain-intrinsic-size`, giving the browser a predictable height to use as a placeholder for the element when it paints.

or another words

> This means it will lay out as if it had a single child of "intrinsic-size" dimensions, ensuring that your unsized divs still occupy space.

### Code example

```
.className {
  content-visibility: auto;
  contain-intrinsic-size: 1000px; /* Height as placeholder. */
}
```


## Result of implementation 
![Result of using 'content-visibility'](https://i0.wp.com/css-tricks.com/wp-content/uploads/2021/06/A460107B-EC0F-46F4-9D1B-CC8461B28F33.jpeg?resize=1000%2C693&ssl=1)


### Constituent properties

* `content-visibility: visible`
* `content-visibility: hidden`
* `content-visibility: auto`
* `contain-intrinsic-size: px`