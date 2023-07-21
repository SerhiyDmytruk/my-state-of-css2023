## [scrollbar-gutter](https://developer.mozilla.org/en-US/docs/Web/CSS/scrollbar-gutter)

[css-tricks](https://css-tricks.com/almanac/properties/s/scrollbar-gutter/) Good examples

> The `scrollbar-gutter` CSS property allows authors to reserve space for the scrollbar, preventing unwanted layout changes as the content grows while also avoiding unnecessary visuals when scrolling isn't needed.

### Code example

```
/* Initial value */
scrollbar-gutter: auto;

/* "stable" keyword, with optional modifier */
scrollbar-gutter: stable;
scrollbar-gutter: stable both-edges;

/* Global values */
scrollbar-gutter: inherit;
scrollbar-gutter: initial;
scrollbar-gutter: revert;
scrollbar-gutter: revert-layer;
scrollbar-gutter: unset;

```
## Result of implementation 

![Examples from css-tricks](https://i0.wp.com/css-tricks.com/wp-content/uploads/2018/11/scrollbar-02.gif?ssl=1)


### Constituent properties

`auto`
> The initial value. Classic scrollbars create a gutter when `overflow` is `scroll`, or when overflow is auto and the box is overflowing. Overlay scrollbars do not consume space.

________________

`stable`
> When using classic scrollbars, the gutter will be present if `overflow` is `auto`, `scroll`, or `hidden` even if the box is not overflowing. When using overlay scrollbars, the gutter will not be present.

________________

`both-edges`
> If a gutter would be present on one of the inline start/end edges of the box, another will be present on the opposite edge as well.