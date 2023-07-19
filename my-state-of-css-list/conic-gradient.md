## [conic-gradient](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/conic-gradient)

> The `conic-gradient()` CSS function creates an image consisting of a gradient with color transitions rotated around a center point (rather than radiating from the center). Example conic gradients include pie charts and color wheels. The result of the conic-gradient() function is an object of the <gradient> data type, which is a special kind of <image>.

### Code example

```
/* A conic gradient rotated 45 degrees,
   starting blue and finishing red */
conic-gradient(from 45deg, blue, red);
conic-gradient(#fff 90deg, #000 0.25turn 0.5turn, #fff 1rad 1.5rad, #000 300grad);
conic-gradient(red .8rad, yellow .6rad, blue 1.3rad);


/* A bluish purple box: the gradient goes from blue to red,
   but only the bottom right quadrant is visible, as the
   center of the conic gradient is at the top left corner */
conic-gradient(from 90deg at 0 0, blue, red);

/* Color wheel */
background: conic-gradient(
    hsl(360, 100%, 50%),
    hsl(315, 100%, 50%),
    hsl(270, 100%, 50%),
    hsl(225, 100%, 50%),
    hsl(180, 100%, 50%),
    hsl(135, 100%, 50%),
    hsl(90, 100%, 50%),
    hsl(45, 100%, 50%),
    hsl(0, 100%, 50%)
);
```
## Result of implementation 

<iframe class="interactive is-default-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/css/function-conic-gradient.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>