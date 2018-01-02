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