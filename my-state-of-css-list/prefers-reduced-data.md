## [prefers-reduced-data](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-data)

> The `prefers-reduced-data` CSS media feature is used to detect if the user has requested the web content that consumes less internet traffic.

### Code example

```
  /* Stuff for reduced data preferences */
@media (prefers-reduced-data: no-preference) {}

  /* Stuff for no data preferences */
@media (prefers-reduced-data: reduce) {}
```