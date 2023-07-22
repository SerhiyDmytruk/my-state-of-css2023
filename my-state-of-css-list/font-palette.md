## [font-palette](https://developer.mozilla.org/en-US/docs/Web/CSS/font-palette)

[font-palette](https://css-tricks.com/colrv1-and-css-font-palette-web-typography/) Good explanation and very deep investigation of that CSS property

> The `font-palette` CSS property allows specifying one of the many palettes contained in a font that a user agent should use for the font. Users can also override the values in a palette or create a new palette by using the [@font-palette-values](font-palette-values.md) at-rule.

### Code example

```
/* Using a font-defined palette */
font-palette: normal;

/* Using a user-defined palette */
font-palette: --one;

```
## Result of implementation 


### Constituent properties

`normal`
> Specifies the default color palette or the default glyph colorization (set by the font maker) to be used for the font. With this setting, the palette in the font at index 0 is rendered.

`light`
> Specifies the first palette in the font that matches 'light' to be used for the font. Some fonts contain metadata that identify a palette as applicable for a light (close to white) background. If a font does not have this metadata, the `light` value behaves as `normal`.

`dark`
> Specifies the first palette in the font that matches 'dark' to be used for the font. Some fonts contain metadata that identify a palette as applicable for a dark (close to black) background. If a font does not have this metadata, the value behaves as `normal`.

`<palette-identifier>`
> Allows you to specify your own values for the font palette by using the [@font-palette-values](font-palette-values.md) at-rule. This value is specified using the <dashed-ident> format.