<img src="http://corysimmons.github.io/elf/img/elf.svg" height="120px">

**Prefer [SCSS](https://github.com/jakecleary/elf-scss)?**

# Elf is now deprecated. Please use https://github.com/corysimmons/lost instead.

### Features
- Unlimited nesting with consistently sized gutters.
- Nesting **without** parent contexts. For instance in Jeet you have to write `column(1/3 1/2)` where `1/2` is the size of the containing element. All ratio grid systems aside from Elf suffer from this in some form or fashion.
- Ratio based sizing (e.g. `column(1/3)`.
- Gutters can be any unit (e.g. `30px`, `2rem`, etc.). These are static so you can space elements vertically as well for a perfect grid.
- Tiny file size compared to other ratio grid systems.
- Flexbox makes short work of aligning elements vertically and horizontally.

#### CodePens
- [Forkable](http://codepen.io/corysimmons/pen/dPParo)
- [Importable](http://codepen.io/corysimmons/pen/qEEgvW)
- [Collection of Examples](http://codepen.io/collection/nLKJkX/)

#### Installation
- Copy and paste [elf.styl](elf.styl) to your project
- `@import 'path/to/elf'`

#### API

(view [elf.styl](elf.styl) for mixin and parameter descriptions)
- `debug(color = blue)`
- `column(ratio = 1, gutter = elf.gutter)`
- `cycle(item = 0, uncycle = 0, gutter = elf.gutter)`
- `offset(ratio = 0, column = true, gutter = elf.gutter)`
- `span(ratio = 1)`
- `shift(ratio = 1, column = true, gutter = elf.gutter)`
- `unshift()`
- `align-children(direction = both)`

#### Browser Support
- General http://caniuse.com/#search=calc
- `align()` http://caniuse.com/#search=flexbox
