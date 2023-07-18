## [CSS containment](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_containment#size_containment)

> explanThe aim of the CSS containment module is to improve performance of web pages by allowing the browser to isolate a subtree of the page from the rest of the page. If the browser knows that a part of the page is independent, rendering can be optimized and performance improved.ation

> In addition, it lets developers indicate whether or not an element should render its contents at all, and whether it should render its contents when it is offscreen. This allows the user agent to apply containment on elements when appropriate, and potentially defer layout and rendering until it is actually needed.


### Key concepts and terminology

```
article {
  contain: content;
}
```

> Each article is independent of the other articles on the page, and so they have been given `contain: content` to indicate to the browser that this is the case. The browser can then use this information to make decisions about how to render the content. For example, it might not render articles that are outside the viewable area.

> If we give each `<article>` the `contain` property with a value of content, when new elements are inserted the browser does not need to recalculate layout or repaint any area outside of the containing element's subtree. If the `<article>` is styled such that its size depends on its contents (e.g. with `height: auto`), then the browser may need to account for its size changing.

___

```
article {
  contain: layout;
}
```

> Layout is normally scoped to the entire document, which means that if you move one element the entire document needs to be treated as if things could have moved anywhere. 

> By using `contain: layout` you can tell the browser it only needs to check this element — everything inside the element is scoped to that element and does not affect the rest of the page, and the containing box establishes an independent formatting context.

___

```
article {
  contain: paint;
}
```

> Paint containment essentially clips the box to the padding edge of the principal box. There can be no visible overflow. The same things are true for `paint` containment as `layout` containment (see above).

> Another advantage is that if the containing box is offscreen, the browser does not need to paint its contained elements — these must also be offscreen as they are contained completely by that box.

___

```
article {
  contain: size;
}
```

> Size containment does not offer much in the way of performance optimizations when used on its own. However, it means that the size of the element's children cannot affect the size of the element itself — its size is computed as if it had no children.

> If you turn on `contain: size` you need to also specify the size of the element you have applied this to using [contain-intrinsic-size](my-state-of-css-list/contain-intrinsic-size.md) (or the equivalent longhand properties). It will end up being zero-sized in most cases, if you don't manually give it a size.

___

```
article {
  contain: style;
}
```

> Despite the name, style containment does not provide scoped styles such as you would get with the Shadow DOM. The main use case is to prevent situations where a CSS Counter could be changed in an element, which could then affect the rest of the tree.

> Using `contain: style` would ensure that the [counter-increment](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-increment) and [counter-set](https://developer.mozilla.org/en-US/docs/Web/CSS/counter-set) properties created new counters scoped to that subtree only.
___

#### Special values

* `content`
* `strict`