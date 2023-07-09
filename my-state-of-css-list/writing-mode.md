## [writing-mode](https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode)

> The `writing-mode` CSS property sets whether lines of text are laid out horizontally or vertically, as well as the direction in which blocks progress. When set for an entire document, it should be set on the root element (html element for HTML documents).

### Code example
```
<style>
.example.Text1 span,
.example.Text1 {
  writing-mode: horizontal-tb;
}

.example.Text2 span,
.example.Text2 {
  writing-mode: vertical-lr;
}

.example.Text3 span,
.example.Text3 {
  writing-mode: vertical-rl;
}

.example.Text4 span,
.example.Text4 {
  writing-mode: sideways-lr;
}

.example.Text5 span,
.example.Text5 {
  writing-mode: sideways-rl;
}


<table>
  <tr>
    <th>Value</th>
    <th>Vertical script</th>
    <th>Horizontal (LTR) script</th>
    <th>Horizontal (RTL) script</th>
    <th>Mixed script</th>
  </tr>
  <tr>
    <td>horizontal-tb</td>
    <td class="example Text1"><span>我家没有电脑。</span></td>
    <td class="example Text1"><span>Example text</span></td>
    <td class="example Text1"><span>מלל ארוך לדוגמא</span></td>
    <td class="example Text1"><span>1994年に至っては</span></td>
  </tr>
  <tr>
    <td>vertical-lr</td>
    <td class="example Text2"><span>我家没有电脑。</span></td>
    <td class="example Text2"><span>Example text</span></td>
    <td class="example Text2"><span>מלל ארוך לדוגמא</span></td>
    <td class="example Text2"><span>1994年に至っては</span></td>
  </tr>
  <tr>
    <td>vertical-rl</td>
    <td class="example Text3"><span>我家没有电脑。</span></td>
    <td class="example Text3"><span>Example text</span></td>
    <td class="example Text3"><span>מלל ארוך לדוגמא</span></td>
    <td class="example Text3"><span>1994年に至っては</span></td>
  </tr>
  <tr>
    <td>sideways-lr</td>
    <td class="example Text4"><span>我家没有电脑。</span></td>
    <td class="example Text4"><span>Example text</span></td>
    <td class="example Text4"><span>מלל ארוך לדוגמא</span></td>
    <td class="example Text4"><span>1994年に至っては</span></td>
  </tr>
  <tr>
    <td>sideways-rl</td>
    <td class="example Text5"><span>我家没有电脑。</span></td>
    <td class="example Text5"><span>Example text</span></td>
    <td class="example Text5"><span>מלל ארוך לדוגמא</span></td>
    <td class="example Text5"><span>1994年に至っては</span></td>
  </tr>
</table>

```

## Result of implementation all writing-modes values

> `sideways-` - at the moment it is impossible to see the result without enabling the settings in your browser, so below is the result of implementing all values

![Result of using 'writing-mode'](https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode/screenshot_2020-02-05_21-04-30.png)
