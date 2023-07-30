## [Open-props](https://github.com/argyleink/open-props)

> Supercharged CSS variables

### Code example 

```
blockquote {
  --_accent-1: var(--lime-5);
  --_accent-2: var(--lime-4);
  --_bg: var(--surface-2);
  --_ink: var(--text-1);

  color: var(--_ink);
  border-color: var(--_accent-2);
  background-color: var(--_bg);
  justify-self: flex-start;
}
```

```
.yellow-badge {
  padding-inline: var(--size-1);
  border-width: var(--border-size-1);
  border-color: var(--yellow-6);
  color: var(--yellow-2);
  border-radius: var(--radius-round);

  @nest [data-theme="light"] & {
    border-color: var(--orange-2);
    color: var(--orange-6);
  }
}
```