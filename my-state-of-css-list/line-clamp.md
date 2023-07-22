## [line-clamp](https://css-tricks.com/almanac/properties/l/line-clamp/)

> The `line-clamp` property truncates text at a specific number of lines.

### Code example

```
.module {
  line-clamp: [none | <integer>];
}
```
## Result of implementation 

```
.line-clamp {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;  
  overflow: hidden;
}
```
<iframe allowfullscreen="true" allowpaymentrequest="true" allowtransparency="true" class="cp_embed_iframe " frameborder="0" height="400" width="100%" name="cp_embed_2" scrolling="no" src="https://codepen.io/geoffgraham/embed/PewgjE?height=400&amp;theme-id=1&amp;slug-hash=PewgjE&amp;default-tab=result&amp;user=geoffgraham&amp;embed-version=2&amp;pen-title=line-clamp%20(-webkit)&amp;name=cp_embed_2" style="width: 100%; overflow: hidden; display: block; height: 400px;" title="line-clamp (-webkit)" loading="lazy" id="cp_embed_PewgjE"></iframe>