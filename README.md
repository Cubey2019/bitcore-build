# vertcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install vertcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var vertcoreTasks = require('vertcore-build');

vertcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var vertcoreTasks = require('vertcore-build');
vertcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/Cubey2019/vertcore) on the main vertcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/Cubey2019/vertcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2017 Cubey2019.

