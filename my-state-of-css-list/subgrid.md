## [Subgrid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout/Subgrid)

> Level 2 of the CSS Grid Layout specification includes a subgrid value for `grid-template-columns` and `grid-template-rows`. This guide details what subgrid does, and gives some use cases and design patterns that are solved by the feature.

### Code example
```
<style>

.grid {
    border: 2px solid #f76707;
    border-radius: 5px;
    background-color: #fff4e6;
}

.item {
    border: 2px solid #ffa94d;
    border-radius: 5px;
    background-color: #ffd8a8;
    color: #d9480f;
}

.subitem {
    background-color: rgb(40, 240, 83);
}

.grid {
    display: grid;
    grid-template-columns: repeat(9, 1fr);
    grid-template-rows: repeat(4, minmax(100px, auto));
}

.item {
    display: grid;
    grid-column: 2 / 7;
    grid-row: 2 / 4;
    grid-template-columns: subgrid;
    grid-template-rows: repeat(3, 80px);
}

.subitem {
    grid-column: 3 / 6;
    grid-row: 1 / 3;
}
</style>

<div class="grid">
  <div class="item">
    <div class="subitem"></div>
  </div>
</div>
    
```


## Result of implementation 
<pre>
  <code>
    <style>
        .grid {
            border: 2px solid #f76707;
            border-radius: 5px;
            background-color: #fff4e6;
        }

        .item {
            border: 2px solid #ffa94d;
            border-radius: 5px;
            background-color: #ffd8a8;
            color: #d9480f;
        }

        .subitem {
            background-color: rgb(40, 240, 83);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(9, 1fr);
            grid-template-rows: repeat(4, minmax(100px, auto));
        }

        .item {
            display: grid;
            grid-column: 2 / 7;
            grid-row: 2 / 4;
            grid-template-columns: subgrid;
            grid-template-rows: repeat(3, 80px);
        }

        .subitem {
            grid-column: 3 / 6;
            grid-row: 1 / 3;
        }
    </style>
    <div class="grid">
        <div class="item">
            <div class="subitem"></div>
        </div>
    </div>
  </code>
</pre>
