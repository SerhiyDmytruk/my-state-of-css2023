## [counter-increment](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-increment)

> The `counter-increment` CSS property increases or decreases the value of a CSS counter by a given value.

### Code example

```
/* Increment "my-counter" by 1 */
counter-increment: my-counter;

/* Decrement "my-counter" by 1 */
counter-increment: my-counter -1;

/* Increment "counter1" by 1, and decrement "counter2" by 4 */
counter-increment: counter1 counter2 -4;

/* Do not increment/decrement anything: used to override less specific rules */
counter-increment: none;

/* Global values */
counter-increment: inherit;
counter-increment: initial;
counter-increment: revert;
counter-increment: revert-layer;
counter-increment: unset;
```
## Result of implementation 

<iframe class="interactive is-default-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/css/counter-increment.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>