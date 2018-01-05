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