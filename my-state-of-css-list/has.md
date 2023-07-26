## [:has()](https://developer.mozilla.org/en-US/docs/Web/CSS/:has)

> The functional `:has()` CSS pseudo-class represents an element if any of the relative selectors that are passed as an argument match at least one element when anchored against this element.


The `:has()` pseudo-class cannot be nested within another `:has()`.

### Code example

```
h1:has(+ p) {}

/* gives the same result as: Serhii remarks */
h1 ~ p {}

```
## Result of implementation 

```
h1,
h2 {
  margin: 0 0 1rem 0;
}

h1:has(+ h2) {
  margin: 0 0 0.25rem 0;
}

:is(h1, h2, h3):has(+ :is(h2, h3, h4)) {
  margin: 0 0 0.25rem 0;
}

```
