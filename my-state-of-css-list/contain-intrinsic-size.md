## [contain-intrinsic-size](https://developer.mozilla.org/en-US/docs/Web/CSS/contain-intrinsic-size)

[w3.org](https://www.w3.org/TR/css-sizing-3/#intrinsic-sizes) Spec
[Intrinsic Sizing In CSS](https://ishadeed.com/article/intrinsic-sizing-in-css/)

> `Intrinsic sizing` determines sizes based on the contents of an element, without regard for its context.


### Code example

```

width: min-content | max-content;


/* Keyword values */
contain-intrinsic-width: none;

/* <length> values */
contain-intrinsic-size: 1000px;
contain-intrinsic-size: 10rem;

/* width | height */
contain-intrinsic-size: 1000px 1.5em;

/* auto <length> */
contain-intrinsic-size: auto 300px;

/* auto width | auto height */
contain-intrinsic-size: auto 300px auto 4rem;

/* Global values */
contain-intrinsic-size: inherit;
contain-intrinsic-size: initial;
contain-intrinsic-size: revert;
contain-intrinsic-size: revert-layer;
contain-intrinsic-size: unset;

```
## Result of implementation 
![Result of implementation `Intrinsic`](https://ishadeed.com/assets/intrinsic-sizing/intrinsic-sizing-1.png)

### Constituent properties
* `contain-intrinsic-width`
* `contain-intrinsic-height`