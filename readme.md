# Skillet
A grid system to end all grid systems, from the team at [Mixd](http://www.mixd.co.uk).

Skillet is based on the amazing work from Nicolas Gallagher's awesome [Griddle](https://github.com/necolas/griddle).

- Flexibility: Complete control to fit it into your own workflow or framework.
- Modular: Defaults to a BEM structured Grid System
- Configurable: Ability to change any class names, gutter sizes or alignment declarations to your hearts desire.
- Lightweight: With its opt-in columns, you're looking at around 5kb minified and gzipped.

## Installation

Skillet is available through a number of package managers, including:

```sh
npm install --save-dev skillet
bower install --save skillet
gem install --save skillet
```

Alternatively, you could always download/clone this repo and use it in your own way.

## Usage

If you've used [Griddle](https://github.com/necolas/griddle) before, you'll see that the syntax is the exact same, if not, don't fear. Skillet is pretty easy to get to grips with.

Once you've imported to the Skillet system, use the `skillet` mixin provided to build out the grids you need.

```scss
@import "skillet";
@include skillet($columns, $extension);
```

It takes two parameters:

- `$columns`: A space-separated list of integers, each of which results in the build of that particular grid.
- `$suffix`: The suffix for the class. This is optional and is intended when you're setting up Skillet instance within a Media Query.


## Configuration
While Skillet may have defaults for the configuration, you still have a lot of freedom in how you'd like to setup your version.

Each of the following variables should be declared **above** the import of Skillet.

**For example:**

```scss
// Alter Config here
@import "skillet";
// Include mixin here
```

**Available options and defaults:**

```scss
// Namespace Options
$skil-grid: "grid";             // The Grid's class namespace.
$skil-item: "grid__item";       // Grid Item's class namespace.
$skil-unit: "grid__item";       // Grid Unit's class namespace.

// Sizing
$skil-gutter: 1em;              // The space between each Grid Item.

// Grid alignment
$skil-grid-direction: inherit;  // Controls the *direction* CSS property for the Grid.
$skil-grid-align-x: inherit;    // Controls the *text-align* property for the Grid.

// Item alignment
$skil-item-direction: inherit;  // Controls the *direction* CSS property for the Grid Item.
$skil-item-align-x: inherit;    // Controls the *text-align* property for the Grid Item.
$skil-item-align-y: top;        // Controls the *vertical-align* property for the Grid Item.
```

## Modifiers


## Examples


## Credits

This framework is under constant development by the [Mixd](http://mixd.co.uk) team. Like it? Hate it? Let us know on [Twitter](http://twitter.com/mixd).

If – like us – you work with WordPress then you may be interested in our other Open Source project called [wp-deploy](https://github.com/Mixd/wp-deploy) a capistrano-powered deployment tool for WordPress.
