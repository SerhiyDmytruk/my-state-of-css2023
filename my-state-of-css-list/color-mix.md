## [color-mix](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/color-mix)

[spec](https://www.w3.org/TR/css-color-5/)

> The `color-mix()` functional notation takes two `<color>` values and returns the result of mixing them in a given colorspace by a given amount.

### Code example

```
color-mix(in lch, plum, pink);
color-mix(in lch, plum 40%, pink);
color-mix(in srgb, #34c9eb 20%, white);
color-mix(in hsl longer hue, hsl(120 100% 50%) 20%, white);

```
## Result of implementation 
<style>
.color-mix li:nth-child(1) {
  background-color: color-mix(in srgb, #34c9eb 0%, white);
}

.color-mix li:nth-child(2) {
  background-color: color-mix(in srgb, #34c9eb 25%, white);
}

.color-mix li:nth-child(3) {
  background-color: color-mix(in srgb, #34c9eb 50%, white);
}

.color-mix li:nth-child(4) {
  background-color: color-mix(in srgb, #34c9eb 75%, white);
}

.color-mix li:nth-child(5) {
  background-color: color-mix(in srgb, #34c9eb 100%, white);
}

.color-mix li:nth-child(6) {
  background-color: color-mix(in srgb, #34c9eb, white);
}


.color-one {
  background-color: hsl(10 100% 50%);
}
.color-two {
  background-color: hsl(60 100% 50%);
}
.shorter {
  background-color: color-mix(
    in hsl shorter hue,
    hsl(10 100% 50%),
    hsl(60 100% 50%)
  );
}
.longer {
  background-color: color-mix(
    in hsl longer hue,
    hsl(10 100% 50%),
    hsl(60 100% 50%)
  );
}


</style>

<ul class="color-mix">
  <li>0%</li>
  <li>25%</li>
  <li>50%</li>
  <li>75%</li>
  <li>100%</li>
  <li></li>
</ul>

<div class="color-one">color one</div>
<div class="color-two">color two</div>
<div class="shorter">mixed shorter</div>
<div class="longer">mixed longer</div>

### Constituent properties