# fresh-css
CSS starter kit with some useful patterns for new projects.

## Layouts

Most of the layouts are based directly on the ones in [Heydon Pickering](https://twitter.com/heydonworks) and [Andy Bell](https://twitter.com/andybelldesign)’s [Every Layout](https://every-layout.dev).

### Box

### Center

### Cluster

### Cover

### Float

### Frame

### Grid

### Reel

### Sidebar

### Stack

### Switcher

## Components

### CTA (Call to Action)

### Responsive Table

## Utilities

### .u-clear-list-style

### .u-reorder-first

### .u-text-center

## Custom Properties

### --gap-flow
**Unit:** `<length>`

**Supported in:** Standard flow layout

Consistent vertical spacing between children inside any flow element (doesn't work on custom
layouts). Inherits to all children.

### --gap-flow-self
**Unit:** `<length>`

**Supported in:** Standard flow layout

Variant of `--gap-flow` that only applies to the current element (doesn't inherit).

### --*__gap (--l-sidebar__gap, etc.)
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Float, Grid, Sidebar, Stack, Switcher

Consistent spacing between children inside the element (or in the case of Float, between the
floated element and nearby elements). Applies to both block and inline axes.

### --*__gap-block (--l-sidebar__gap-block, etc.)
**Unit:** `<length>`

**Supported in:** Cluster, Cover, Float, Grid, Sidebar, Stack, Switcher

Block-only `--*__gap`.

### --*__gap-inline (--l-sidebar__gap-inline, etc.)
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Float, Grid, Sidebar, Switcher

Inline-only `--*__gap`.

### --*__gutter (--l-box__gutter, etc.)
**Unit:** `<length>`

**Supported in:** Box, Cover

Consistent padding along the edges of an element.

### --*__breakpoint (--l-box-switcher__breakpoint, etc.)
**Unit:** `<length>`

**Supported in:** Float, Sidebar, Switcher

Sets the breakpoint at which the layout switches from a side-by-side style to a vertical stacked
style. When available, it's better to use the numbered `--breakpoint-*` properties, since they
apply depending on the number of children in the layout. However, some layouts, such as Float, only
support the single `--breakpoint` value.

### --*__max-size (--l-center__max-size, etc.)
**Unit:** `<length>`

**Supported in:** Center, Float

The maximum size of an element along its primary axis (as determined by the layout or component).
For Center this refers to the width of the centered element, while for Float it refers to the
width of the floated element.

### --*__min-size (--l-cover__min-size, etc.)
**Unit:** `<length>`

**Supported in:** Cover, Float, Sidebar

The minimum size of an element along its primary axis (as determined by the layout or component).
For Cover this refers to the height of the entire layout, while for Sidebar it refers to the main
content item and for Float it refers to the width of the floated element.

### --l-float__direction
**Unit:** `left|right`

**Supported in:** Float

The direction to align the layout. Passed directly to the `float` property.

### --l-frame__aspect-ratio
**Unit:** `<number>/<number>`

**Supported in:** Frame

A fractional aspect ratio in the format "x/y".
