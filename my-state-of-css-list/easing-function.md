## [Easing Function](https://www.w3.org/TR/css-easing-1/#easing-function)

> An easing function takes an [input progress value](https://www.w3.org/TR/css-easing-1/#input-progress-value) and produces an [output progress value](https://www.w3.org/TR/css-easing-1/#output-progress-value).

> An [easing function](https://www.w3.org/TR/css-easing-1/#easing-function) must be a pure function meaning that for a given set of inputs, it always produces the same [output progress value](https://www.w3.org/TR/css-easing-1/#output-progress-value).


### Code example

```
<easing-function> = linear | <cubic-bezier-easing-function> | <step-easing-function>
```


### Constituent properties

[The linear easing function: `linear`](https://www.w3.org/TR/css-easing-1/#the-linear-easing-function)

>The **linear easing function** is an identity function meaning that its output progress value is equal to the input progress value for all inputs.

> The syntax for the linear easing function is simply the `linear` keyword.

[Cubic Bézier easing functions: ease, ease-in, ease-out, ease-in-out, cubic-bezier()](https://www.w3.org/TR/css-easing-1/#cubic-bezier-easing-functions)

>A **cubic Bézier easing function** is a type of easing function defined by four real numbers that specify the two control points, P1 and P2, of a cubic Bézier curve whose end points P0 and P3 are fixed at (0, 0) and (1, 1) respectively. The x coordinates of P1 and P2 are restricted to the range [0, 1].

![cubic Bézier easing function](https://www.w3.org/TR/css-easing-1/images/cubic-bezier-easing-curve.svg ':size=300x300')

[Step easing functions: step-start, step-end, steps()](https://www.w3.org/TR/css-easing-1/#step-easing-functions)

> A **step easing function** is a type of `easing function` that divides the input time into a specified number of intervals that are equal in length. It is defined by a number of **steps**, and a **step position**. It has following syntax: