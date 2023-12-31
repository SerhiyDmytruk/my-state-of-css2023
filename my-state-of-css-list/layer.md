## [@layer](https://developer.mozilla.org/en-US/docs/Web/CSS/@layer)

> The `@layer` CSS at-rule is used to declare a cascade layer and can also be used to define the order of precedence in case of multiple cascade layers.


![Cascade Layers](https://i0.wp.com/css-tricks.com/wp-content/uploads/2021/09/css-cascade-cascade-layers-champ-bramus-1120x630-1.png?resize=1000%2C563&ssl=1)

### Code example

```
@layer layer-name {rules}
@layer layer-name;
@layer layer-name, layer-name, layer-name;
@layer {rules}
```
## Result of implementation 

```
<style>

  .box p {
    color: rebeccapurple;
  }

  @layer type {
    .box-item p {
      font-weight: bold;
      font-size: 1.3em;
      color: green;
    }
  }

</style>


<div class="box">
  <div class="box-item">
    <p>Hello, world!</p>
  </div>
</div>
```

<style>

.box p {
  color: rebeccapurple;
}

@layer type {
  .box-item p {
    font-weight: bold;
    font-size: 1.3em;
    color: green;
  }
}

</style>


<div class="box">
  <div class="box-item">
    <p>Hello, world!</p>
  </div>
</div>


<iframe class="interactive is-tabbed-standard-height" height="400" src="https://interactive-examples.mdn.mozilla.net/pages/tabbed/at-rule-layer.html" title="MDN Web Docs Interactive Example" loading="lazy" data-readystate="complete"></iframe>