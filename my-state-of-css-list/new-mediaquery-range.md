## [The New CSS Media Query Range Syntax](https://css-tricks.com/the-new-css-media-query-range-syntax/)

> Media Queries Level 4 specifies a [new and simpler syntax](https://www.w3.org/TR/mediaqueries-4/#mq-ranges) using less then (<), greater than (>) and equals (=) operators. So, that last example can be converted to the new syntax, like so:


[Syntax improvements in Level 4](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries#syntax_improvements_in_level_4)
> The Media Queries Level 4 specification includes some syntax improvements to make media queries using features that have a "range" type, for example width or height, less verbose. Level 4 adds a range context for writing such queries. For example, using the max- functionality for width we might write the following:

### Code example

```
@media (30em <= width <= 80em) {
  /* ... */
}
```


### Constituent properties
* `<` evaluates if a value is less than another value
* `>` evaluates if a value is greater than another value
* `=` evaluates if a value is equal to another value
* `<=` evaluates if a value is less than or equal to another value
* `>=` evaluates if a value is greater than or equal to another value