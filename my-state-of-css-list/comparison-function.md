## [CSS Comparison Functions clamp(), max() and min()](https://dev.to/ekaterina_vu/css-comparison-functions-clamp-max-and-min-4aon)

> `clamp(min, val | preffered, max)`

> The `clamp()` CSS function clamps a middle value within a range of values between a defined minimum bound and a maximum bound. The function takes three parameters: a minimum value, a preferred value, and a maximum allowed value.

```
/* Static values */
width: clamp(200px, 40%, 400px);
width: clamp(20rem, 30vw, 70rem);
width: clamp(10vw, 20em, 100vw);

/* Calculated values */
width: clamp(min(10vw, 20rem), 300px, max(90vw, 55rem));
width: clamp(100px, calc(30% / 2rem + 10px), 900px);

```

<iframe height="600" src="https://codepen.io/Ekaterina_Vu/embed/QWjxJvm?height=600&amp;default-tab=result&amp;embed-version=2" scrolling="no" frameborder="no" allowtransparency="true" loading="lazy" style="width: 100%;">
</iframe>

_________________________________________

**Note**: both `min()` and `max()` can be replaced with `max-width` or `min-width` if the element has width property and only two parameters are passed into the function. 
It sounds a bit counterintuitive, but `max()` actually sets the lower size limit and `min()` the upper size limit.

___________________________________________

`max()`
> Function `max()` calculates and applies the largest value from the provided range of values. 


```
/* max() */
.element {
   width: max(50vw, 500px);
}
/* gives the same result as: */
.element {
    width: 50vw;
    min-width: 500px;
}

```
<iframe class="interactive is-default-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/css/function-max.html" title="Інтерактивний приклад MDN Web Docs" loading="lazy" data-readystate="complete"></iframe>

_____________________________

`min()`
> Likewise, function `min()` calculates and applies the smallest value from the range. 


```
/* min() */
.element {
    width: min(50vw, 500px);
}
/* gives the same result as: */
.element {
    width: 50vw;
    max-width: 500px;
}
```

<iframe class="interactive is-default-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/css/function-min.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>