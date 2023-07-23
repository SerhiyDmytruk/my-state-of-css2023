## [prefers-contrast](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-contrast)

> The `prefers-contrast` CSS media feature is used to detect whether the user has requested the web content to be presented with a lower or higher contrast.

### Code example

```
@media (prefers-contrast: no-preference) {}

@media (prefers-contrast: more) {}

@media (prefers-contrast: less) {}

@media (prefers-contrast: custom) {}
```

### Constituent properties

`no-preference`
> Indicates that the user has made no preference known to the system. This keyword value evaluates as false in the Boolean context.

`more`
> Indicates that user has notified the system that they prefer an interface that has a higher level of contrast.

`less`
> Indicates that user has notified the system that they prefer an interface that has a lower level of contrast.

`custom`
> Indicates that user has notified the system for using a specific set of colors, and the contrast implied by these colors matches neither more nor less. This value will match the color palette specified by users of `forced-colors: active`.