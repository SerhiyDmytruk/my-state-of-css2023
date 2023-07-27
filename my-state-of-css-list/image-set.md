## [image-set()](https://developer.mozilla.org/en-US/docs/Web/CSS/image/image-set)

> The `image-set()` CSS functional notation is a method of letting the browser pick the most appropriate CSS image from a given set, primarily for high pixel density screens.

### Code example

```
/* Select image based on resolution */
 background-image: image-set(
  "image1.jpg" 1x,
  "image2.jpg" 2x
);

 background-image: image-set(
  url("image1.jpg") 1x,
  url("image2.jpg") 2x
);

/* Select gradient based on resolution */
 background-image: image-set(
  linear-gradient(blue, white) 1x,
  linear-gradient(blue, green) 2x
);

/* Select image based on supported formats */
 background-image: image-set(
  url("image1.avif") type("image/avif"),
  url("image2.jpg") type("image/jpeg")
);

```
## Result of implementation 
<iframe width="100%" height="600" src="https://mdn.github.io/css-examples/images/image-set.html" loading="lazy"></iframe>