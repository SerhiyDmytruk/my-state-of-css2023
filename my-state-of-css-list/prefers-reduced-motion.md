## [prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion)

[prefers-reduced-motion: Sometimes less movement is more](https://web.dev/prefers-reduced-motion/) Article from Google team

> The `prefers-reduced-motion` CSS media feature is used to detect if a user has enabled a setting on their device to minimize the amount of non-essential motion. The setting is used to convey to the browser on the device that the user prefers an interface that removes, reduces, or replaces motion-based animations.

> Such animations can trigger discomfort for those with vestibular motion disorders. Animations such as scaling or panning large objects can be vestibular motion triggers.

### Code example

```
  /* styles to apply if a user's device settings are set to reduced motion */
@media (prefers-reduced-motion: reduce) {}

  /* styles to apply if a user's device settings are set to reduced motion */
@media (prefers-reduced-motion: no-preference) {}

```
## Result of implementation 
<iframe width="560" height="315" src="https://www.youtube.com/embed/uANmA7korfs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>