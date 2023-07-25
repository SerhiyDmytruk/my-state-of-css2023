## [@supports](https://developer.mozilla.org/en-US/docs/Web/CSS/@supports)

> The `@supports` CSS at-rule lets you specify CSS declarations that depend on a browser's support for CSS features. Using this at-rule is commonly called a feature query. The rule must be placed at the top level of your code or nested inside any `other conditional group at-rule`.

`Conditional group rules are`
* @media,
* @supports,
* @document. (deferred to Level 4 of CSS Spec)


### Code example

```
  /* If the condition is true, use the CSS in this block. */
@supports (<supports-condition>) {}


  /* If both conditions are true, use the CSS in this block. */
@supports (<supports-condition>) and | or | not (<supports-condition>) {}


// The conditions can be combined by conjunctions (and), disjunctions (or), and/or negations (not).

@supports (display: table-cell) and (display: list-item) {}

@supports (transform-style: preserve) or (-moz-transform-style: preserve) {}

@supports not (transform-origin: 10em 10em 10em) {}

// combinations
@supports not (not (transform-origin: 2px)) {}
@supports (display: grid) and (not (display: inline-grid)) {}


```

### Constituent properties

`selector()`
> This function evaluates if a browser supports the specified selector syntax. The following example returns true and applies the CSS style if the browser supports the child combinator:

```
@supports selector(h2 > p) {}

```

`font-tech()`
> This function checks if a browser supports the specified font technology for layout and rendering. The following example returns true and applies the CSS style if the browser supports the COLRv1 font technology:

```
@supports font-tech(color-COLRv1) {}

```

`font-format()`
> This function checks if a browser supports the specified font format for layout and rendering. The following example returns true and applies the CSS style if the browser supports the `opentype` font format:

```
@supports font-format(opentype) {}
```