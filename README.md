# fresh-css
CSS starter kit with some useful patterns for new projects.

## Layouts

Most of the layouts are based directly on the ones in [Heydon Pickering](https://twitter.com/heydonworks) and [Andy Bell](https://twitter.com/andybelldesign)’s [Every Layout](https://every-layout.dev).

### Box

### Carousel

### Center

### Cluster

### Cover

### Float

### Frame

### Grid

### Sidebar

### Stack

### Switcher

## Components

### CTA (Call to Action)

### Responsive Table

## Utilities

### center

### clear-list-style

### reorder-first

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

### --gap
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Float, Grid, Sidebar, Stack, Switcher

Consistent spacing between children inside the element (or in the case of Float, between the
floated element and nearby elements). Applies to both block and inline axes.

### --gap-block
**Unit:** `<length>`

**Supported in:** Cluster, Cover, Float, Grid, Sidebar, Stack, Switcher

Block-only `--gap`.

### --gap-inline
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Float, Grid, Sidebar, Switcher

Inline-only `--gap`.

### --gap-inherit
**Values:** `inherit`

**Supported in:** Carousel, Cluster, Cover, Grid, Sidebar, Stack, Switcher

When set to the `inherit` keyword, this property takes on the nearest ancestor gap value. Most
custom layouts use this when computing gaps, since it makes sure the parent and child both have the
same gap value.

### --gap-inherit-block
**Values:** `inherit`

**Supported in:** Carousel, Cluster, Cover, Grid, Sidebar, Stack, Switcher

Block-only `--gap-inherit`.

### --gap-inherit-inline
**Values:** `inherit`

**Supported in:** Carousel, Cluster, Cover, Grid, Sidebar, Stack, Switcher

Inline-only `--gap-inherit`.

### --gutter
**Unit:** `<length>`

**Supported in:** Box, Cover

Consistent padding along the edges of an element.

### --gutter-inherit
**Unit:** `<length>`

**Supported in:** Box, Cover

When set to the `inherit` keyword, this property takes on the nearest ancestor gutter value. The
"Stretch" variant of the Box layout uses this to break out of the gutter of its parent while
still maintaining its own independent gutter value.

### --breakpoint
**Unit:** `<length>`

**Supported in:** Float, Sidebar, Switcher

Sets the breakpoint at which the layout switches from a side-by-side style to a vertical stacked
style. When available, it's better to use the numbered `--breakpoint-*` properties, since they
apply depending on the number of children in the layout. However, some layouts, such as Float, only
support the single `--breakpoint` value.

### --breakpoint-base
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

For elements with multiple responsive breakpoints, this is the starting point for calculating
the breakpoints.

### --breakpoint-scale
**Unit:** `<number>`

**Supported in:** Sidebar, Switcher

For elements with multiple responsive breakpoints, this is the value used for calculating the
modular scale.

### --breakpoint-1
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has one child. Computed using a modular scale by default, but can
be manually overriden.

### --breakpoint-2
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has two children. Computed using a modular scale by default, but
can be manually overriden.

### --breakpoint-3
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has three children. Computed using a modular scale by default, but
can be manually overriden.

### --breakpoint-4
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has four children. Computed using a modular scale by default, but
can be manually overriden.

### --breakpoint-5
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has five children. Computed using a modular scale by default, but
can be manually overriden.

### --breakpoint-6
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has six children. Computed using a modular scale by default, but
can be manually overriden.

### --breakpoint-7-or-more
**Unit:** `<length>`

**Supported in:** Sidebar, Switcher

The breakpoint when the element has seven or more children. Computed using a modular scale by
default, but can be manually overriden.

### --max-size
**Unit:** `<length>`

**Supported in:** Center, Float

The maximum size of an element along its primary axis (as determined by the layout or component).
For Center this refers to the width of the centered element, while for Float it refers to the
width of the floated element.

### --min-size
**Unit:** `<length>`

**Supported in:** Cover, Float, Sidebar

The minimum size of an element along its primary axis (as determined by the layout or component).
For Cover this refers to the height of the entire layout, while for Sidebar it refers to the main
content item and for Float it refers to the width of the floated element.

### --direction
**Unit:** `left|right`

**Supported in:** Float

The direction to align the layout. Passed directly to the `float` property.

### --aspect-ratio
**Unit:** `<number>/<number>`

**Supported in:** Frame

A fractional aspect ratio in the format "x/y".

### --has-gap-left
**Unit:** `0|1`

**Supported in:** Float

If 1, include a gap (in the form of margin) on the left side of the floated element.

### --has-gap-right
**Unit:** `0|1`

**Supported in:** Float

If 1, include a gap (in the form of margin) on the right side of the floated element.

### --aspect-ratio
**Unit:** `<number>/<number>`

**Supported in:** Frame

A fractional aspect ratio in the format "x/y".

### --child-target-size
**Unit:** `<length>`

**Supported in:** Grid, Sidebar

The size that child elements will start at before layout calculation via Flexbox or Grid. Layouts
may selectively apply this property to children. For example, Sidebar only applies it to the
sidebar, not the main content, while Grid applies it to all items.

### --child-target-size-fallback
**Unit:** `<length>`

**Supported in:** Grid

A fallback value for `--child-target-size` in cases where the layout or component uses an
experimental method of setting the size (such as the `min()` function in Grid).

### --target-size
**Unit:** `<length>`

**Supported in:** Sidebar

Same as `--child-target-size`, but for the purpose of overriding the parent value for
specific children.
