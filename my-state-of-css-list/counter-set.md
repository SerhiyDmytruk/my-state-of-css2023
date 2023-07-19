## [counter-set](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-set)

[counter-set](https://css-tricks.com/almanac/properties/c/counter-set/)

> The `counter-set` CSS property sets a CSS counter to a given value. It manipulates the value of existing counters, and will only create new counters if there isn't already a counter of the given name on the element.

### Code example

```
/* Set "my-counter" to 0 */
counter-set: my-counter;

/* Set "my-counter" to -1 */
counter-set: my-counter -1;

/* Set "counter1" to 1, and "counter2" to 4 */
counter-set: counter1 1 counter2 4;

/* Cancel any counter that could have been set in less specific rules */
counter-set: none;

/* Global values */
counter-set: inherit;
counter-set: initial;
counter-set: revert;
counter-set: revert-layer;
counter-set: unset;
```
## Result of implementation 

<iframe class="interactive is-default-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/css/counter-set.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>