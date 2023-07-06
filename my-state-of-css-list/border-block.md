## [Border block](https://developer.mozilla.org/en-US/docs/Web/CSS/border-block)

The `border-block` CSS property is a shorthand property for setting the individual logical block border property values in a single place in the style sheet.

```
<style>
  .border {
    border: 1px solid tomato;
  }

  .border-block {
    border-block: medium dashed tomato;
  }
</style>

<div class="border">
    border
</div>

  <div class="border-block">
    border-block
</div>

```


<pre>
  <code>
      <style>
        .border {
          border: 1px solid tomato;
        }

        .border-block {
          border-block: medium dashed tomato;
        }
      </style>
      <div class="border">
          border
      </div>

        <div class="border-block">
          border-block
      </div>
  </code>
</pre>

### Constituent properties
This property is a shorthand for the following CSS properties:

* `border-block-color`

* `border-block-style`
  * `border-block-style: dashed;`
  * `border-block-style: dotted;`
  * `border-block-style: groove;`


* `border-block-width` same approach as for `border-width`
  * `border-width: thin;`
  * `border-width: medium;`
  * `border-width: thick;`
  * `border-width: NUMBERpx;`
