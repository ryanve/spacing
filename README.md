# spacing
Opensource functional CSS spacing for modern web development

- [<b>setup</b>](#setup)
- [<b>classes</b>](#classes)
- [<b>data-spacing</b>](#data-spacing)
- [<b>scaling</b>](#scaling)
- [<b>files</b>](#files)

## setup

```
npm install spacing
```

### import whichever [file(s)](#files) meets your needs

- [`main.css`](main.css) is harcoded for CSS3 compatibility
- [`module.css`](module.css) uses CSS4 variables

```css
@import "node_modules/spacing/main";
```

## classes
Classes are listed in order from least to most precendence.

### `padding`
- `.p0`
- `.p1`
- `.p2`
- `.p3`
- `.p4`

### `padding-top`
- `.pt0`
- `.pt1`
- `.pt2`
- `.pt3`
- `.pt4`

### `padding-left`
- `.pl0`
- `.pl1`
- `.pl2`
- `.pl3`
- `.pl4`

### `padding-right`
- `.pr0`
- `.pr1`
- `.pr2`
- `.pr3`
- `.pr4`

### `padding-bottom`
- `.pb0`
- `.pb1`
- `.pb2`
- `.pb3`
- `.pb4`

### `margin`
- `.m0`
- `.m1`
- `.m2`
- `.m3`
- `.m4`
- `.m-auto`

### `margin-top`
- `.mt0`
- `.mt1`
- `.mt2`
- `.mt3`
- `.mt4`
- `.mt-auto`

### `margin-left`
- `.ml0`
- `.ml1`
- `.ml2`
- `.ml3`
- `.ml4`
- `.ml-auto`

### `margin-right`
- `.mr0`
- `.mr1`
- `.mr2`
- `.mr3`
- `.mr4`
- `.mr-auto`

### `margin-bottom`
- `.mb0`
- `.mb1`
- `.mb2`
- `.mb3`
- `.mb4`
- `.mb-auto`

### `:first-child`
- `.mt0-first`
- `.ml0-first`
- `.mr0-first`
- `.mb0-first`

### `:last-child`
- `.mt0-last`
- `.ml0-last`
- `.mr0-last`
- `.mb0-last`

## data-spacing

Alternative to [classes](#classes) you can also space via `[data-spacing]` with value(s) being any of the classes.

```html
<p data-spacing="p1 m0 mb2">
```

All `[data-spacing]` selectors come after the classes in the cascade.

## scaling

### spacing variables default to `rem` and therefore can be scaled responsively with the `rem` size

```css
:root {
  font-size: 1em;
  font-size: calc(.9em + .5vw + .5vh);
}
```

### in CSS4 you could scale via media queries

```css
:root {
  --space-1: .5rem;
  --space-2: 1rem;
  --space-3: 1.5rem;
  --space-4: 3rem;
}

@media (min-width: 30em) and (min-height: 20em) {
  :root {
    --space-1: .5rem;
    --space-2: 1rem;
    --space-3: 2rem;
    --space-4: 4rem;
  }
}
```

## files

- [main.css](main.css) css3+ bundle
  - [module.css](module.css) css4+ bundle
    - [class.css](class.css) class selectors
    - [data.css](data.css) data selectors
    - [root.css](root.css) default variables
