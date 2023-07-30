## [Tachyons](https://github.com/tachyons-css/tachyons/)

> Tachyons embraces a different style than many popular CSS frameworks known as "Functional CSS".


### PRINCIPLES

* Everything should be 100% responsive
* Everything should be readable on any device
* Everything should be as fast as possible
* Designing in the browser should be easy
* It should be easy to change any interface or part of an interface without breaking any existing interfaces
* Doing one thing extremely well promotes reusability and reduces repetition
* Documentation helps promote reusability and shared knowledge
* CSS shouldn't impede accessibility or the default functionality of HTML
* You should send the smallest possible amount of code to the user

### Features

* Mobile-first CSS architecture
* 490 accessible color combinations
* 8px baseline grid
* Multiple debugging utilities to reduce layout struggles
* Single-purpose class structure
* Optimized for maximum gzip compression
* Lightweight (~14kB)
* Usable across projects
* Growing open source component library
* Works well with plain HTML, React, Ember, Angular, Rails and more
* Infinitely nestable responsive grid system
* Built with PostCSS


## Tachyons Approach 

Tachyons approaches this with `single utility classes` (classes that do one thing).
These `single utility classes` encourage a different way of building UI:
all code is in a single place the `html`, not the `stylesheet`:

```
<button class="bw0 br2 bg-dwyl-teal pa2 white fw1 tc ttu tracked">do what you love</button>
```

**Note**: Tachyons does not have all-the-colors, hence we had to define our own. However given that there is a clear format for defining colors we defined our own as `bg-dwyl-teal`:

```
.bg-dwyl-teal {
  background-color: #4DB6AC;
}
```

### What is "Functional" CSS?

Functional CSS is:
* Functional
> Small, clear, easy to read classes that are easy to apply and do one thing.
Having small classes means it's easy to make a set of **consistent spacing and type rules** - you end up forcing a beautiful type scale & rhythm on your design.

* Composable
> In Functional Programming you combine (or compose) a bunch of tiny functions together to do bigger things (like lots of notes to make music!). You end up reusing a lot of your code which is great for **performance and consistency**! Just like the button example:

* Immutable
> In Functional languages declaring a property means it will never get overwritten, something known as Immutability - i.e it can't ever be changed (or mutated). A huge benefit you gain from immutability is that code is easier to reason about (you **don't have to** go on a **hunt** to find where something might have been changed