## [Semantic-UI && Fomantic-UI](https://github.com/semantic-org/semantic-ui)

> Semantic is a development framework that helps create beautiful, responsive layouts using human-friendly HTML.


### Concise HTML

Semantic UI treats words and classes as exchangeable concepts.

Classes use syntax from natural languages like noun/modifier relationships, word order, and plurality to link concepts intuitively.

Get the same benefits as BEM or SMACSS, but without the tedium.


```
<div class="ui three buttons">
  <button class="ui active button">One</button>
  <button class="ui button">Two</button>
  <button class="ui button">Three</button>
</div>
```
## Intuitive Javascript 
Semantic uses simple phrases called behaviors that trigger functionality.

Any arbitrary decision in a component is included as a setting that developers can modify.

```
$('select.dropdown')
  .dropdown('set selected', ['meteor', 'ember'])
;

<select name="skills" multiple="" class="ui fluid dropdown">
  <option value="">Skills</option>
  <option value="angular">Angular</option>
  <option value="css">CSS</option>
  <option value="ember">Ember</option>
  <option value="html">HTML</option>
  <option value="javascript">Javascript</option>
  <option value="meteor">Meteor</option>
  <option value="node">NodeJS</option>
</select>
```

### Simplified Debugging

Performance logging lets you track down bottlenecks without digging through stack traces.