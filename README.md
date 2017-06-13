# spacing
Opensource functional CSS spacing for modern web development

## setup

```
npm install spacing
```

Use either the [main](main.css) or [module](module.css) file based on your needs. The main file uses harcoded sensible spacing values. The module is configurable with CSS variables and good for developing but must be built in your pipeline for deep browser support. Import both if you want to have live CSS variables in the browser but fallback to hardcoded values.

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

## scaling

Spacing variables default to using `rem` such that you can scale them with the `rem` size to make a responsive system.

```css
:root {
  font-size: 1em;
  font-size: calc(.9em + .5vw + .5vh);
}
```
