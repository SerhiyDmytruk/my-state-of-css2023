## [touch-action](https://developer.mozilla.org/en-US/docs/Web/CSS/touch-action)

> The `touch-action` CSS property sets how an element's region can be manipulated by a touchscreen user (for example, by zooming features built into the browser).


### Code example

```
/* Keyword values */
touch-action: auto;
touch-action: none;
touch-action: pan-x;
touch-action: pan-left;
touch-action: pan-right;
touch-action: pan-y;
touch-action: pan-up;
touch-action: pan-down;
touch-action: pinch-zoom;
touch-action: manipulation;

/* Global values */
touch-action: inherit;
touch-action: initial;
touch-action: revert;
touch-action: revert-layer;
touch-action: unset;

```

### Constituent properties

`auto`
> Enable browser handling of all panning and zooming gestures.

> A declaration of `touch-action: none;` may inhibit operating a browser's zooming capabilities. This will prevent people experiencing low vision conditions from being able to read and understand page content.

__________________

`none`
> Disable browser handling of all panning and zooming gestures.

__________________

`pan-x`
> Enable single-finger horizontal panning gestures. May be combined with **pan-y, pan-up, pan-down** and/or **pinch-zoom**.

__________________

`pan-y`
> Enable single-finger vertical panning gestures. May be combined with **pan-x, pan-left, pan-right** and/or **pinch-zoom**.
__________________


`manipulation`
> Enable panning and pinch zoom gestures, but disable additional non-standard gestures such as double-tap to zoom. Disabling double-tap to zoom removes the need for browsers to delay the generation of **click** events when the user taps the screen. This is an alias for **"pan-x pan-y pinch-zoom"** (which, for compatibility, is itself still valid).

__________________


`pan-left, pan-right, pan-up, pan-down`
> Enable single-finger gestures that begin by scrolling in the given direction(s). Once scrolling has started, the direction may still be reversed. Note that scrolling "up" (pan-up) means that the user is dragging their finger downward on the screen surface, and likewise pan-left means the user is dragging their finger to the right. Multiple directions may be combined except when there is a simpler representation (for example, **"pan-left pan-right"** is invalid since **"pan-x"** is simpler, but **"pan-left pan-down"** is valid).

__________________


`pinch-zoom`
> Enable multi-finger panning and zooming of the page. This may be combined with any of the **pan-** values.