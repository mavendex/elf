# calc-grid

### Installation
Just add this mixin to your Stylus stylesheet anywhere.

```stylus
col(ratio = 1, cycle = 0, gutter = 30px)
  float: left
  width: s('calc(100% * %s - %s + %s * %s)', ratio, gutter, ratio, gutter)
  margin-right: gutter
  &:nth-child({cycle}n), &:last-child
    margin-right: 0
```

### Syntax
`col(ratio, cycle, gutter)`

### Usage
Want 3 columns?

```html
<div>block</div>
<div>block</div>
<div>block</div>
```

```stylus
div
  col(1/3)
```

Want to add more elements and have them drop to next row automatically?

```html
<div>block</div>
<div>block</div>
<div>block</div>
<div>block</div>
<div>block</div>
```

```stylus
div
  col(1/3, 3)
```

Prefer no gutters?

```stylus
div
  col(1/3, 3, 0)
```

### Browser Support
http://caniuse.com/#search=calc
