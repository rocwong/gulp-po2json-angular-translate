# gulp-po2json-angular-translate

> gulp plugin to convert po to angangular-translate format
> 
> based on [grunt-po2json-angular-translate v0.0.3](https://github.com/angular-translate/grunt-po2json-angular-translate)

## Install

Install with [npm](https://npmjs.org/package/gulp-angular-gettext)

```sh
npm install gulp-po2json-angular-translate --save-dev
```

## Example

```js
var gulp = require('gulp');
var po2json = require('gulp-po2json-angular-translate');
gulp.task('po2jsjon', function () {
  return gulp.src('po/**/*.po')
    .pipe(po2json({
    	// options ...
    	pretty: false
    }))
    .pipe(gulp.dest('dist/translations/'));
});
```

## Options

### options.pretty
Type: `Boolean`
Default value:  `false`
If you want to pretty print the result


### options.upperCaseId
Type: `Boolean`
Default value:  `false`
If you want to convert the ids to uppercase


### options.enableAltPlaceholders
Type: `Boolean`
Default value:  `true`
It enables you to use alternative placeholders format, it defaults with {foo}.

### options.placeholderStructure
Type: `Array`
Default value:  `['{','}']`
Here you can set your own placeholder structure. Notice that you must specify a closing mark.


## More
See [grunt-po2json-angular-translate](https://github.com/angular-translate/grunt-po2json-angular-translate)