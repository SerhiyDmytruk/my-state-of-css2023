## [object-view-box](https://css-tricks.com/first-look-at-the-css-object-view-box-property/)

> with `object-view-box` we can essentially draw the image boundaries as we can [with an SVG’s viewbox](https://css-tricks.com/scale-svg/#aa-the-viewbox-attribute). So, take a plain ol’ `<img>` and call on `object-view-box` to trim the edges using an inset function

### Code example

```
img {
    aspect-ratio: 1;
    width: 300px;
    object-view-box: inset(25% 20% 15% 0%);
    object-fit: cover;
}
```
## Result of implementation 

<iframe height="900" style="width: 100%;" scrolling="no" title="CSS object-view-box" src="//codepen.io/anon/embed/yLvXJRd?height=900&theme-id=1&slug-hash=yLvXJRd&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/shadeed/pen/yLvXJRd">
  CSS object-view-box</a> by Ahmad Shadeed (<a href="https://codepen.io/shadeed">@shadeed</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>


### Constituent properties

* `object-view-box`
* `object-fit`