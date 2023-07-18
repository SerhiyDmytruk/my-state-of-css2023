## [backdrop-filter](https://developer.mozilla.org/en-US/docs/Web/CSS/backdrop-filter?retiredLocale=uk)

> The `backdrop-filter` CSS property lets you apply graphical effects such as blurring or color shifting to the area behind an element. Because it applies to everything behind the element, to see the effect you must make the element or its background at least partially transparent.

### Code example

```
<style>
.box {
  background-color: rgb(255 255 255 / 0.3);
  backdrop-filter: blur(10px);
  position: relative;
  top: 50%;
  left: 0;
  height: 50px;
}

.container {
  background-image: url("../img/plumeria.jpg");
  width: 400px;
  height: 400px;
}
</style>

<div class="container">
  <div class="box">
    <p>backdrop-filter: blur(10px)</p>
  </div>
</div>

```
## Result of implementation 
<style>
.box {
  background-color: rgb(255 255 255 / 0.3);
  backdrop-filter: blur(10px);
  position: relative;
  top: 50%;
  left: 0;
  height: 50px;
}

.container {
  background-image: url("../img/plumeria.jpg");
  width: 400px;
  height: 400px;
}
</style>

<div class="container">
  <div class="box">
    <p>backdrop-filter: blur(10px)</p>
  </div>
</div>

<iframe class="interactive is-default-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/css/backdrop-filter.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>

### Constituent properties
```
/* Keyword value */
backdrop-filter: none;

/* URL to SVG filter */
backdrop-filter: url(commonfilters.svg#filter);

/* <filter-function> values */
backdrop-filter: blur(2px);
backdrop-filter: brightness(60%);
backdrop-filter: contrast(40%);
backdrop-filter: drop-shadow(4px 4px 10px blue);
backdrop-filter: grayscale(30%);
backdrop-filter: hue-rotate(120deg);
backdrop-filter: invert(70%);
backdrop-filter: opacity(20%);
backdrop-filter: sepia(90%);
backdrop-filter: saturate(80%);

/* Multiple filters */
backdrop-filter: url(filters.svg#filter) blur(4px) saturate(150%);

/* Global values */
backdrop-filter: inherit;
backdrop-filter: initial;
backdrop-filter: revert;
backdrop-filter: revert-layer;
backdrop-filter: unset;

```