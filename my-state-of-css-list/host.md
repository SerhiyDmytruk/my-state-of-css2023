## [:host()](https://developer.mozilla.org/en-US/docs/Web/CSS/:host_function)

> The `:host()` CSS pseudo-class function selects the shadow host of the shadow DOM containing the CSS it is used inside (so you can select a custom element from inside its shadow DOM) — but only if the selector given as the function's parameter matches the shadow host.


### Code example

```
/* Selects a shadow root host, only if it is
   matched by the selector argument */
:host(.special-custom-element) {}

```
## Result of implementation 

<iframe class="interactive is-tabbed-shorter-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/tabbed/pseudo-class-host_function.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>