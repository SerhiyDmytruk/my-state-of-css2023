## [:slotted()](https://developer.mozilla.org/en-US/docs/Web/CSS/::slotted)

> The `::slotted()` CSS pseudo-element represents any element that has been placed into a slot inside an HTML template (see Using templates and slots for more information).

This only works when used inside CSS placed within a shadow DOM. Note also that this selector won't select a text node placed into a slot; it only targets actual elements.


### Code example

```
/* Selects any element placed inside a slot */
::slotted(*) {}

/* Selects any <span> placed inside a slot */
::slotted(span) {}

```
## Result of implementation 


<iframe class="interactive is-tabbed-shorter-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/tabbed/pseudo-element-slotted.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>