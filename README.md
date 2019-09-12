# fresh-css
CSS starter kit with some useful patterns for new projects.

## Layouts

Most of the layouts are based directly on the ones in [Heydon Pickering](https://twitter.com/heydonworks) and [Andy Bell](https://twitter.com/andybelldesign)’s [Every Layout](https://every-layout.dev).

### Box

### Carousel

### Center

### Cluster

### Cover

### Frame

### Grid

### Sidebar

### Stack

### Switcher

## Components

### Responsive Table

## Utilities

### center

### clear-list-style

### reorder-first

## Custom Properties

### --gap
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Grid, Sidebar, Stack, Switcher

Consistent spacing between children inside the element. Applies to both block and inline axes.

### --gap-block
**Unit:** `<length>`

**Supported in:** Cluster, Cover, Grid, Sidebar, Stack, Switcher

Block-only `--gap`.

### --gap-inline
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Grid, Sidebar, Switcher

Inline-only `--gap`.

### --gap-self
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Sidebar, Stack, Switcher

Overrides the inherited `--gap` value for a single element without affecting its children.

### --gap-block-self
**Unit:** `<length>`

**Supported in:** Cluster, Cover, Sidebar, Stack, Switcher

Overrides the inherited `--gap-block` value for a single element without affecting its children.

### --gap-inline-self
**Unit:** `<length>`

**Supported in:** Carousel, Cluster, Cover, Sidebar, Switcher

Overrides the inherited `--gap-inline` value for a single element without affecting its children.

### --gutter
**Unit:** `<length>`

**Supported in:** Box, Cover

Consistent padding along the edges of an element.

### --breakpoint-base
**Unit:** `<length>`

**Supported in:** Switcher

For elements with multiple responsive breakpoints, this is the starting point for calculating the breakpoints.

### --breakpoint-scale
**Unit:** `<number>`

**Supported in:** Switcher

For elements with multiple responsive breakpoints, this is the value used for calculating the modular scale.

### --breakpoint-1
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has one child. Computed using a modular scale by default, but can be manually overriden.

### --breakpoint-2
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has two children. Computed using a modular scale by default, but can be manually overriden.

### --breakpoint-3
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has three children. Computed using a modular scale by default, but can be manually overriden.

### --breakpoint-4
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has four children. Computed using a modular scale by default, but can be manually overriden.

### --breakpoint-5
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has five children. Computed using a modular scale by default, but can be manually overriden.

### --breakpoint-6
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has six children. Computed using a modular scale by default, but can be manually overriden.

### --breakpoint-7-or-more
**Unit:** `<length>`

**Supported in:** Switcher

The breakpoint when the element has seven or more children. Computed using a modular scale by default, but can be manually overriden.

### --max-size
**Unit:** `<length>`

**Supported in:** Center

The maximum size of an element along its primary axis (as determined by the layout or component).

### --min-size
**Unit:** `<length>`

**Supported in:** Cover

The minimum size of an element along its primary axis (as determined by the layout or component).

### --aspect-ratio
**Unit:** `<number>/<number>`

**Supported in:** Frame

A fractional aspect ratio in the format "x/y".

### --child-target-size
**Unit:** `<length>`

**Supported in:** Grid, Sidebar

The size that child elements will start at before layout calculation via Flexbox or Grid. Layouts may selectively apply this property to children. For example, Sidebar only applies it to the sidebar, not the main content, while Grid applies it to all items.

### --child-target-size-fallback
**Unit:** `<length>`

**Supported in:** Grid

A fallback value for `--child-target-size` in cases where the layout or component uses an experimental method of setting the size (such as the `min()` function in Grid).
