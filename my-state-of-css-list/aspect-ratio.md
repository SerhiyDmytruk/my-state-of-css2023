## aspect-ratio

> The `aspect-ratio` CSS property sets a preferred aspect ratio for the box, which will be used in the calculation of auto sizes and some other layout functions.

### Code example

```
<style>
  .output {
    padding: 0;
    margin: 0;
  }

  .output li {
    float: left;
    display: flex;
    justify-content: center;
    width: 300px;
    height: 300px;
    overflow: hidden;
    text-align: center;
  }

  img {
    max-width: initial;
    height: 100%;
    width: auto;
    flex-grow: 0;
  }

  .aspect-ratio-auto {
    aspect-ratio: auto;
  }

  .aspect-ratio-1-1 {
    aspect-ratio: 1 / 1;
  }

  .aspect-ratio-16-9 {
    aspect-ratio: 16 / 9;
  }

  .aspect-ratio-0-5 {
    aspect-ratio: 0.5;
  }
</style>

<ul>
  <li>
      <img class="aspect-ratio-auto" src="./img/plumeria.jpg" alt="flower"/>
  </li>
  <li>
      <img class="aspect-ratio-1-1" src="./img/plumeria.jpg" alt="flower"/>
  </li>
  <li>
      <img class="aspect-ratio-16-9" src="./img/plumeria.jpg" alt="flower"/>
  </li>
  <li>
      <img class="aspect-ratio-0-5" src="./img/plumeria.jpg" alt="flower"/>
  </li>
</ul>
```

## Result of implementation 


  <style>
    .output {
      padding: 0!important;
      margin: 0;
    }

    .output li {
      float: left;
      display: flex;
      justify-content: center;
      width: 300px;
      height: 300px;
      overflow: hidden;
      text-align: center;
    }

    img {
      max-width: initial!important;
      height: 100%;
      width: auto;
      flex-grow: 0;
    }

    .aspect-ratio-auto {
      aspect-ratio: auto;
    }

    .aspect-ratio-1-1 {
      aspect-ratio: 1 / 1;
    }

    .aspect-ratio-16-9 {
      aspect-ratio: 16 / 9;
    }

    .aspect-ratio-0-5 {
      aspect-ratio: 0.5;
    }
  </style>

<ul class="output">
  <li>
      <img class="aspect-ratio-auto" src="./img/plumeria.jpg" alt="flower"/>
  </li>
  <li>
      <img class="aspect-ratio-1-1" src="./img/plumeria.jpg" alt="flower"/>
  </li>
  <li>
      <img class="aspect-ratio-16-9" src="./img/plumeria.jpg" alt="flower"/>
  </li>
  <li>
      <img class="aspect-ratio-0-5" src="./img/plumeria.jpg" alt="flower"/>
  </li>
</ul>