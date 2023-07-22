## [text-wrap](https://developer.mozilla.org/en-US/docs/Web/CSS/text-wrap)

> The `text-wrap` CSS property controls how text inside an element is wrapped. The different values provide:

### Code example

```
/* Keyword values */
text-wrap: wrap;
text-wrap: nowrap;
text-wrap: balance;

/* Global values */
text-wrap: inherit;
text-wrap: initial;
text-wrap: revert;
text-wrap: revert-layer;
text-wrap: unset;

```

### Constituent properties

`wrap`

> Text is wrapped across lines at appropriate characters (for example spaces, in languages like English that use space separators) to minimize overflow. This is the default value.

_____________

`nowrap`

> Text does not wrap across lines. It will overflow its containing element rather than breaking onto a new line.

_____________

`balance`

> Text is wrapped in a way that best balances the number of characters on each line, enhancing layout quality and legibility