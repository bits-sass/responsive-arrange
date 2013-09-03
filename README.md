# Bits.sass responsive arrange

Responsive superset of arrange component.

See [Bits.sass arrange](https://github.com/bits-sass/arrange) for more about
the component itself.

Read more about [Bits.sass toolkit](https://github.com/bits-sass/bits.sass).

## Installation

* __Bower:__ `bower install --save bits-sass-responsive-arrange`
* __Download:__ [zip](https://github.com/bits-sass/responsive-arrange/zipball/master), [tar.gz](https://github.com/bits-sass/responsive-arrange/tarball/master)
* __Git:__ `git clone https://github.com/bits-sass/responsive-arrange.git`

## Available SASS variables

* `bits-components-ns` - components namespace, defaults to 'bits-'
* `bits-responsive-arrange-gutter-sizes` - list of generated gutters

## Available classes

* `v[n]-Arrange` - core component class on `n` breakpoint
* `v[n]-Arrange--middle` - modifier class for middle-aligned cells on `n` breakpoint
* `v[n]-Arrange--bottom` - modifier class for bottom-aligned cells on `n` breakpoint
* `v[n]-Arrange--equal` - modifier class for equal-width cells on `n` breakpoint
* `v[n]-Arrange--gutter` - modifier class for an inter-cell gutter on `n` breakpoint
* `v[n]-Arrange--gutter--small` - (adjustable) gutter of 5px on `n` breakpoint
* `v[n]-Arrange--gutter--medium` - (adjustable) gutter of 10px on `n` breakpoint
* `v[n]-Arrange--gutter--large` - (adjustable) gutter of 20px on `n` breakpoint
* `v[n]-Arrange-sizeFit` - child class for cells to snap to fit their content on `n` breakpoint
* `v[n]-Arrange-sizeFill` - child class for cells to expand to fill the remaining space on `n` breakpoint

## Usage

A grid that turns itself into an arrange component on `v4` breakpoint.

```html
<div class="Grid u-gutterVm v4-Arrange v4-Arrange--middle
  v4-Arrange--gutter v4-Arrange--gutter--medium">
  <div class="Grid-cell v4-Arrange-sizeFill">
    <input type="text">
  </div>
  <div class="Grid-cell v4-Arrange-sizeFit">
    <button class="Button Button--primary">Send</button>
  </div>
</div>
```

## Requirements

* Sass 3.2+

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 9+ (IE 8 requires a build step)