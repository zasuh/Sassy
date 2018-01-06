## Getting Sassy with CSS ##

### December 31st 2017 ###
- Websites are getting complex and CSS isn't enough.
- Lots of repetition is happening with CSS.
- The main mission of SASS is to remove this repetition using nesting, variables, better selectors, mixins, inline imports and so on.
- *Compiling SASS*: `$ sass source_dir output_dir`
- *Running SASS*: `$ sass sass/application.scss css/application.css`
- *Watching in SASS*: `$ sass --watch source.scss:output.css`
- *Compile `source.css` to `output.css`*: `$ sass --update source.scss:output.css`

### January 1st 2018 ###
- Same as HTML nesting, we can nest in SASS.
- Use SASS to orginize and to get rid of repetition.
- As a general recommendation it is good to not go more than 3 layers deep.
- Sass allows us to reference the *current parent selector(s)* via the *ampersand* (&) character.

### January 2nd 2018 ###
- `@import` means another files download. It includes the source during compilation time.
- Files with underscores create partials. They don't compile to `.css` files and allow us to maintain code in more modular chunks.

### January 3rd 2018 ###
- *Variables* are probably most associated with colors, font sizes, font families, font paths, padding, margins, border and all other properties that tend to be repeated.
- `$grey: rgba(0,0,0,.5);` is later referenced: `color: $grey`.
- *Data types* consist of integers, strings, color, lists, booleans, null and maps.
- Variables can be injected at later times using: `${variable_name}`

### January 4th 2018 ###
- Manipulating colors with math: `#555555 + #112233; // => #667788`

### January 5th 2018 ###
- Mixins allow the reuse of block styles.
- Instead of just one single value bind to a variable name, we can add more values to a name with `@mixin` followed by the mixin name.
- We can then `@include` mixins when needed.

### January 6th 2018 ###
- `@extends` lets us group selectors together.
- `%` is used with placeholders.
- In SASS you declare functions with `@function` and return values with `@return` other than that they work like normal functions, taking arguments, running a bit of code and returning values.
- Same goes for `@if` and `@else` statements, `@each`, `@for`, `@while`.
- *Maps* give us key-value pairings. I've associated them with objects, where each key has some value assigned to them, in the case of CSS it's color, font families and so on.
- You can nest *Media Queries* under any declaration in SASS. You can use variables to assign breakpoints.
- *Modular Architecture* is the abstraction of repetition into "objects". This means thinking in modules with various states, knowing when to use classes vs. using IDs and having good naming convetions. Modularity, scalability, maintainability, not repeating ourselves and staying organized are goals when it comes to modular architecture.
- *Compass* a CSS Authoring Framework. *Bourbon* a simple and lightweight mixin library for SASS. *Susy* which adds responsive grids to Compass.
- Extensively use modules, don't extend too much, mind your mixins and media queries, check your output and enable SASS sourcemaps for debugging.