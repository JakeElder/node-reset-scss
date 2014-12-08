Node Reset SCSS
===============

A simple node module for including Eric Meyer's reset css as a sass partial

## Usage with Gulp:

```
var gulp = require('gulp');
var sass = require('gulp-sass');

gulp.task('sass', function () {
  gulp.src('path/to/input.scss')
    .pipe(sass({
      includePaths: require('node-reset-scss').includePath
    }))
    .pipe(gulp.dest('path/to/output.css'));
});
```

