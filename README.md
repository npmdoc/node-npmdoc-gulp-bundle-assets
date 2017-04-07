# api documentation for  [gulp-bundle-assets (v2.27.1)](https://github.com/dowjones/gulp-bundle-assets#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-bundle-assets.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-bundle-assets) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-bundle-assets.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-bundle-assets)
#### Create asset (js, css) bundles from a config file leveraging the power of streams

[![NPM](https://nodei.co/npm/gulp-bundle-assets.png?downloads=true)](https://www.npmjs.com/package/gulp-bundle-assets)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-bundle-assets_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Montgomery",
        "url": "http://www.chrismontgomery.info/"
    },
    "bugs": {
        "url": "https://github.com/dowjones/gulp-bundle-assets/issues"
    },
    "contributors": [
        {
            "name": "Chris Montgomery",
            "url": "http://www.chrismontgomery.info/"
        },
        {
            "name": "Christian Sherland",
            "url": "https://github.com/csherland"
        },
        {
            "name": "Roberto Soares",
            "url": "https://github.com/roberto"
        },
        {
            "name": "bas",
            "url": "https://github.com/21brains-zh"
        },
        {
            "name": "gregorymaertens",
            "url": "https://github.com/gregorymaertens"
        },
        {
            "name": "narthollis",
            "url": "https://github.com/narthollis"
        },
        {
            "name": "PlasmaPower",
            "url": "https://github.com/PlasmaPower"
        }
    ],
    "dependencies": {
        "bluebird": "3.3.5",
        "duplexer2": "0.0.2",
        "graceful-fs": "4.1.4",
        "gulp": "3.9.1",
        "gulp-clean-css": "2.0.7",
        "gulp-coffee": "2.3.2",
        "gulp-concat": "2.5.2",
        "gulp-if": "2.0.1",
        "gulp-less": "3.1.0",
        "gulp-order": "1.1.1",
        "gulp-rev": "4.0.0",
        "gulp-sourcemaps": "1.5.2",
        "gulp-streamify": "0.0.5",
        "gulp-uglify": "1.5.3",
        "gulp-util": "3.0.7",
        "lazypipe": "0.2.3",
        "lodash": "3.9.3",
        "map-stream": "0.0.6",
        "merge-stream": "0.1.7",
        "mkdirp": "0.5.1",
        "pretty-hrtime": "1.0.2",
        "readable-stream": "2.0.0",
        "through2": "2.0.1",
        "vinyl": "1.1.1"
    },
    "description": "Create asset (js, css) bundles from a config file leveraging the power of streams",
    "devDependencies": {
        "browserify": "10.2.4",
        "coveralls": "2.11.2",
        "gulp-help": "1.6.0",
        "gulp-istanbul": "0.10.0",
        "gulp-istanbul-enforcer": "1.0.3",
        "gulp-jshint": "1.11.0",
        "gulp-mocha": "2.1.1",
        "gulp-nice-package": "1.0.0",
        "gulp-sass": "2.0.4",
        "gulp-shrinkwrap": "2.0.1",
        "jshint-stylish": "2.0.0",
        "mocha-lcov-reporter": "0.0.2",
        "multiline": "1.0.2",
        "proxyquire": "1.5.0",
        "rimraf": "^2.5.2",
        "should": "6.0.3",
        "sinon": "1.15.3",
        "vinyl-source-stream": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "2e837c15ea9cbd3ac9fdcde5b214234cb75d84f8",
        "tarball": "https://registry.npmjs.org/gulp-bundle-assets/-/gulp-bundle-assets-2.27.1.tgz"
    },
    "gitHead": "3c4b9fadb149b4d401dc51666f7f1b2b3895afd1",
    "homepage": "https://github.com/dowjones/gulp-bundle-assets#readme",
    "keywords": [
        "gulp",
        "gulpfriendly",
        "bundle",
        "bundles",
        "bundling",
        "assets",
        "asset",
        "combine",
        "compress",
        "minify",
        "minification",
        "package",
        "static",
        "resource",
        "javascript",
        "css"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "chmontgomery",
            "email": "chr.montgomery@gmail.com"
        }
    ],
    "name": "gulp-bundle-assets",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dowjones/gulp-bundle-assets.git"
    },
    "scripts": {
        "coveralls": "gulp test-cover && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage",
        "test": "gulp ci"
    },
    "version": "2.27.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-bundle-assets](#apidoc.module.gulp-bundle-assets)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.</span>results (opts)](#apidoc.element.gulp-bundle-assets.results)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.</span>watch (opts)](#apidoc.element.gulp-bundle-assets.watch)
1.  object <span class="apidocSignatureSpan">gulp-bundle-assets.</span>stream_files
1.  object <span class="apidocSignatureSpan">gulp-bundle-assets.</span>string_helper
1.  object <span class="apidocSignatureSpan">gulp-bundle-assets.</span>transformHelper
1.  object <span class="apidocSignatureSpan">gulp-bundle-assets.</span>using

#### [module gulp-bundle-assets.stream_files](#apidoc.module.gulp-bundle-assets.stream_files)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>attachStreamOptions (file, opts)](#apidoc.element.gulp-bundle-assets.stream_files.attachStreamOptions)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>handleTransformError (thisStream, isWatch, bundleName, bundleKey, err)](#apidoc.element.gulp-bundle-assets.stream_files.handleTransformError)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>scripts (opts)](#apidoc.element.gulp-bundle-assets.stream_files.scripts)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>styles (opts)](#apidoc.element.gulp-bundle-assets.stream_files.styles)

#### [module gulp-bundle-assets.string_helper](#apidoc.module.gulp-bundle-assets.string_helper)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.string_helper.</span>endsWith (str, suffix)](#apidoc.element.gulp-bundle-assets.string_helper.endsWith)

#### [module gulp-bundle-assets.transformHelper](#apidoc.module.gulp-bundle-assets.transformHelper)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.transformHelper.</span>browserify (func)](#apidoc.element.gulp-bundle-assets.transformHelper.browserify)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.transformHelper.</span>coffee (opts)](#apidoc.element.gulp-bundle-assets.transformHelper.coffee)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.transformHelper.</span>less (opts)](#apidoc.element.gulp-bundle-assets.transformHelper.less)

#### [module gulp-bundle-assets.using](#apidoc.module.gulp-bundle-assets.using)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.using.</span>bundle (key, type, env, bundleAllEnvironments)](#apidoc.element.gulp-bundle-assets.using.bundle)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.using.</span>bundleName (key, type, env, bundleAllEnvironments)](#apidoc.element.gulp-bundle-assets.using.bundleName)
1.  [function <span class="apidocSignatureSpan">gulp-bundle-assets.using.</span>copy (base)](#apidoc.element.gulp-bundle-assets.using.copy)



# <a name="apidoc.module.gulp-bundle-assets"></a>[module gulp-bundle-assets](#apidoc.module.gulp-bundle-assets)

#### <a name="apidoc.element.gulp-bundle-assets.results"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.</span>results (opts)](#apidoc.element.gulp-bundle-assets.results)
- description and source-code
```javascript
results = function (opts) {
  var resultJsons = {},
    resultOrder,
    options = defaulOptions(opts);

  function collectResults(file, enc, cb) {
    addBundleResults(resultJsons, file, options.pathPrefix, options.fileName);
    if (!resultOrder) {
      try {
        resultOrder = file.bundle.result.bundleOrder; // Any one of these properties could be null
      } catch (err) {}
    }
    this.push(file);
    cb();
  }

  function writeResults(done) {
    mkdirp(options.dest, function (err) {
      if (err) throw err;

      var streams = [];

      _.each(resultJsons, function (result) {
        var sortedContents = {};
        try {
          // order bundle names based on original bundle.config.js ordering
          _.each(resultOrder || Object.keys(result.contents), function (key) {
            // order scripts/styles for consistency
            var sortedBundleTypes = {};
            _.each(Object.keys(result.contents[key]).sort(), function (typeKey) {
              sortedBundleTypes[typeKey] = result.contents[key][typeKey];
            });
            sortedContents[key] = sortedBundleTypes;
          });
        } catch (err) { // any problems sorting? just fall back to what we get out of the stream
          sortedContents = result.contents;
        }
        var filePath = path.join(options.dest, result.filename),
          data = JSON.stringify(sortedContents, null, 2);
        streams.push(fs.writeFileAsync(filePath, data));
      });

      bluebird.all(streams).then(function () {
        done();
      });

    });
  }

  return through.obj(collectResults, writeResults);
}
```
- example usage
```shell
...
// gulpfile.js
var gulp = require('gulp'),
  bundle = require('gulp-bundle-assets');

gulp.task('bundle', function() {
  return gulp.src('./bundle.config.js')
    .pipe(bundle())
    .pipe(bundle.results('./')) // arg is destination of bundle.result.json
    .pipe(gulp.dest('./public'));
});
'''

Which results in a 'bundle.result.json' file similar to:

'''json
...
```

#### <a name="apidoc.element.gulp-bundle-assets.watch"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.</span>watch (opts)](#apidoc.element.gulp-bundle-assets.watch)
- description and source-code
```javascript
watch = function (opts) {
  var configFile,
    config;
  opts = opts || {};
  if (!opts.configPath) {
    throw new gutil.PluginError('gulp-bundle-assets', 'configPath option is required when watching');
  }
  if (!opts.dest) {
    throw new gutil.PluginError('gulp-bundle-assets', 'dest option is required when watching');
  }

  try {
    configFile = require(opts.configPath);
    config = new ConfigModel(configFile, opts);
  } catch (e) {
    gutil.log(e);
    throw new gutil.PluginError('gulp-bundle-assets', 'Failed to parse config file');
  }

  cache.set('config', config);

  streamBundlesWatch(config);
}
```
- example usage
```shell
...
        if (scriptWatch !== false) {

          scriptsPath = pathifySrc(namedBundleObj[BundleKeys.SCRIPTS], base, namedBundleObj[BundleKeys.OPTIONS], env);
          prettyScriptsBundleName = using.bundleName(bundleName, BundleKeys.SCRIPTS, env, isBundleAll);

          logger.log("Starting '" + gutil.colors.cyan("watch") + "' for bundle '" + gutil.colors.green(prettyScriptsBundleName) + "'...");

          gulp.watch((typeof scriptWatch === 'string' || util.isArray(scriptWatch)) ? scriptWatch : scriptsPath)
            .on('change', function (file) { // log changed file?

var start = process.hrtime();

streamFiles.scripts({
  src: scriptsPath,
  base: base,
...
```



# <a name="apidoc.module.gulp-bundle-assets.stream_files"></a>[module gulp-bundle-assets.stream_files](#apidoc.module.gulp-bundle-assets.stream_files)

#### <a name="apidoc.element.gulp-bundle-assets.stream_files.attachStreamOptions"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>attachStreamOptions (file, opts)](#apidoc.element.gulp-bundle-assets.stream_files.attachStreamOptions)
- description and source-code
```javascript
attachStreamOptions = function (file, opts) {
  // add some useful options to file for possible inspection later in external custom gulp streams
  file.bundleOptions = {
    env: opts.env,
    type: opts.type,
    bundleName: opts.bundleName,
    isWatch: opts.isWatch,
    isBundleAll: opts.isBundleAll
  };
}
```
- example usage
```shell
...
  concatOpts = defaults({
    path: opts.bundleName + ((opts.isBundleAll && opts.env) ? '.' + opts.env : '') + '.js'
  }, opts.bundleOptions.pluginOptions['gulp-concat']);

return gulp.src(opts.src, {base: opts.base})
  .pipe(using.bundle(opts.bundleName, BundleKeys.SCRIPTS, opts.env, opts.isBundleAll))
  .pipe(through.obj(function (file, enc, cb) {
    self.attachStreamOptions(file, opts);
    this.push(file);
    cb();
  }))
  .pipe(gif(function (file) {
      return sourcemaps.isEnabled(opts);
    }, gsourcemaps.init(opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.SCRIPTS].init)
  ))
...
```

#### <a name="apidoc.element.gulp-bundle-assets.stream_files.handleTransformError"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>handleTransformError (thisStream, isWatch, bundleName, bundleKey, err)](#apidoc.element.gulp-bundle-assets.stream_files.handleTransformError)
- description and source-code
```javascript
handleTransformError = function (thisStream, isWatch, bundleName, bundleKey, err) {
  logger.log(gutil.colors.red("ERROR in custom transforms for '" + bundleName + "." + bundleKey + "':"));
  logger.log(err.toString());
  if (isWatch) {
    thisStream.emit('end');
  } else {
    process.exit(1);
  }
}
```
- example usage
```shell
...
}))
.pipe(gif(function (file) {
    return sourcemaps.isEnabled(opts);
  }, gsourcemaps.init(opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.SCRIPTS].init)
))
.pipe(opts.bundleOptions.transforms[BundleKeys.SCRIPTS]())
.on('error', function (e) {
  self.handleTransformError(this, opts.isWatch, opts.bundleName, BundleKeys.SCRIPTS, e);
})
.pipe(gif(function (file) {
    return sourcemaps.isEnabled(opts);
  }, through.obj(sourcemaps.verify)
))
.pipe(gif(function (file) {
    return isMinEnabled.js(file, opts);
...
```

#### <a name="apidoc.element.gulp-bundle-assets.stream_files.scripts"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>scripts (opts)](#apidoc.element.gulp-bundle-assets.stream_files.scripts)
- description and source-code
```javascript
scripts = function (opts) {
  var self = this,
    concatOpts = defaults({
      path: opts.bundleName + ((opts.isBundleAll && opts.env) ? '.' + opts.env : '') + '.js'
    }, opts.bundleOptions.pluginOptions['gulp-concat']);

  return gulp.src(opts.src, {base: opts.base})
    .pipe(using.bundle(opts.bundleName, BundleKeys.SCRIPTS, opts.env, opts.isBundleAll))
    .pipe(through.obj(function (file, enc, cb) {
      self.attachStreamOptions(file, opts);
      this.push(file);
      cb();
    }))
    .pipe(gif(function (file) {
        return sourcemaps.isEnabled(opts);
      }, gsourcemaps.init(opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.SCRIPTS].init)
    ))
    .pipe(opts.bundleOptions.transforms[BundleKeys.SCRIPTS]())
    .on('error', function (e) {
      self.handleTransformError(this, opts.isWatch, opts.bundleName, BundleKeys.SCRIPTS, e);
    })
    .pipe(gif(function (file) {
        return sourcemaps.isEnabled(opts);
      }, through.obj(sourcemaps.verify)
    ))
    .pipe(gif(function (file) {
        return isMinEnabled.js(file, opts);
      },
      gif(function (file) {
          return file.isStream();
        },
        streamify(
          uglify(opts.bundleOptions.pluginOptions['gulp-uglify'])),
        uglify(opts.bundleOptions.pluginOptions['gulp-uglify'])
      )))
    .on('error', function (e) {
      self.handleTransformError(this, opts.isWatch, opts.bundleName, BundleKeys.SCRIPTS, e);
    })
    .pipe(gif(function (file) {
        return opts.bundleOptions.order && opts.bundleOptions.order.scripts;
      }, order(opts.bundleOptions.order.scripts)
    ))
    .pipe(gif(function (file) {
        return file.isStream();
      },
      streamify(concat(concatOpts)),
      concat(concatOpts)
    ))
    .pipe(gif(isOptionEnabled(opts.bundleOptions.rev, opts.env),
      gif(function (file) {
        return file.isStream();
      }, streamify(rev()), rev())
    ))
    .pipe(gif(function (file) {
        return sourcemaps.isEnabled(opts);
      }, gsourcemaps.write(
        opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.SCRIPTS].destPath,
        opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.SCRIPTS].write
      )
    ))
    .pipe(addBundleResultsToFile(opts.bundleName, BundleKeys.SCRIPTS, opts.bundleOptions.result, opts.env, opts.isBundleAll, opts
.bundleOrder));
}
```
- example usage
```shell
...
          logger.log("Starting '" + gutil.colors.cyan("watch") + "' for bundle '" + gutil.colors.green(prettyScriptsBundleName) + "'...");

          gulp.watch((typeof scriptWatch === 'string' || util.isArray(scriptWatch)) ? scriptWatch : scriptsPath)
            .on('change', function (file) { // log changed file?

var start = process.hrtime();

streamFiles.scripts({
  src: scriptsPath,
  base: base,
  env: env,
  type: type,
  bundleName: bundleName,
  bundleOptions: namedBundleObj[BundleKeys.OPTIONS],
  isBundleAll: isBundleAll,
...
```

#### <a name="apidoc.element.gulp-bundle-assets.stream_files.styles"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.stream_files.</span>styles (opts)](#apidoc.element.gulp-bundle-assets.stream_files.styles)
- description and source-code
```javascript
styles = function (opts) {
  var self = this;
  return gulp.src(opts.src, {base: opts.base})
    .pipe(using.bundle(opts.bundleName, BundleKeys.STYLES, opts.env, opts.isBundleAll))
    .pipe(through.obj(function (file, enc, cb) {
      self.attachStreamOptions(file, opts);
      this.push(file);
      cb();
    }))
    .pipe(
    gif(function (file) {
        return sourcemaps.isEnabled(opts);
      }, gsourcemaps.init(opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.STYLES].init)
    ))
    .pipe(opts.bundleOptions.transforms[BundleKeys.STYLES]())
    .on('error', function (e) {
      self.handleTransformError(this, opts.isWatch, opts.bundleName, BundleKeys.STYLES, e);
    })
    .pipe(gif(function (file) {
        return sourcemaps.isEnabled(opts);
      }, through.obj(sourcemaps.verify)
    ))
    .pipe(gif(function (file) {
      return isMinEnabled.css(file, opts);
    }, cleanCSS(opts.bundleOptions.pluginOptions['gulp-clean-css'])))
    .pipe(gif(function (file) {
        return opts.bundleOptions.order && opts.bundleOptions.order.styles;
      }, order(opts.bundleOptions.order.styles)
    ))
    .pipe(concat(opts.bundleName + ((opts.isBundleAll && opts.env) ? '.' + opts.env : '') + '.css'))
    .pipe(gif(isOptionEnabled(opts.bundleOptions.rev, opts.env), rev()))
    .pipe(gif(function (file) {
        return sourcemaps.isEnabled(opts);
      }, gsourcemaps.write(
        opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.STYLES].destPath,
        opts.bundleOptions.pluginOptions['gulp-sourcemaps'][BundleKeys.STYLES].write
      )
    ))
    .pipe(addBundleResultsToFile(opts.bundleName, BundleKeys.STYLES, opts.bundleOptions.result, opts.env, opts.isBundleAll, opts
.bundleOrder));
}
```
- example usage
```shell
...
          logger.log("Starting '" + gutil.colors.cyan("watch") + "' for bundle '" + gutil.colors.green(prettyStylesBundleName) + "'...");

          gulp.watch((typeof styleWatch === 'string' || util.isArray(styleWatch)) ? styleWatch : stylesPath)
            .on('change', function (file) { // log changed file?

var start = process.hrtime();

streamFiles.styles({
  src: stylesPath,
  base: base,
  env: env,
  type: type,
  bundleName: bundleName,
  bundleOptions: namedBundleObj[BundleKeys.OPTIONS],
  isBundleAll: isBundleAll,
...
```



# <a name="apidoc.module.gulp-bundle-assets.string_helper"></a>[module gulp-bundle-assets.string_helper](#apidoc.module.gulp-bundle-assets.string_helper)

#### <a name="apidoc.element.gulp-bundle-assets.string_helper.endsWith"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.string_helper.</span>endsWith (str, suffix)](#apidoc.element.gulp-bundle-assets.string_helper.endsWith)
- description and source-code
```javascript
endsWith = function (str, suffix) {
  if (typeof str !== 'string' || typeof suffix !== 'string') {
    throw new Error('stringHelper.endsWith expected strings but got str "' + str + '" and suffix "' + suffix + '"');
  }
  return str.indexOf(suffix, str.length - suffix.length) !== -1;
}
```
- example usage
```shell
...
    cb();
  });
};

module.exports.copy = function (base) {
  return through.obj(function (file, enc, cb) {
    var pathReplace = (base === '.') ? file.cwd : base;
    if (!stringHelper.endsWith(pathReplace, '/')) {
      pathReplace += '/';
    }
    logger.log("Copy file", gutil.colors.magenta(file.path.replace(pathReplace, '')));
    this.push(file);
    cb();
  });
};
...
```



# <a name="apidoc.module.gulp-bundle-assets.transformHelper"></a>[module gulp-bundle-assets.transformHelper](#apidoc.module.gulp-bundle-assets.transformHelper)

#### <a name="apidoc.element.gulp-bundle-assets.transformHelper.browserify"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.transformHelper.</span>browserify (func)](#apidoc.element.gulp-bundle-assets.transformHelper.browserify)
- description and source-code
```javascript
browserify = function (func) {
  return lazypipe()
    .pipe(function () {
      var writable = new readableStream.Writable({objectMode: true});
      var readable = through.obj(function (file, enc, cb) { // noop
        this.push(file);
        cb();
      });

      writable._write = function _write(file, encoding, done) {
        func(file, readable);
        return done();
      };

      return duplexer(writable, readable);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-bundle-assets.transformHelper.coffee"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.transformHelper.</span>coffee (opts)](#apidoc.element.gulp-bundle-assets.transformHelper.coffee)
- description and source-code
```javascript
coffee = function (opts) {
  opts = opts || {};
  return lazypipe()
    .pipe(function () {
      return gif(isCoffeeFile, coffee(opts));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-bundle-assets.transformHelper.less"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.transformHelper.</span>less (opts)](#apidoc.element.gulp-bundle-assets.transformHelper.less)
- description and source-code
```javascript
less = function (opts) {
  opts = opts || {};
  return lazypipe()
    .pipe(function () {
      return gif(isLessFile, less(opts));
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-bundle-assets.using"></a>[module gulp-bundle-assets.using](#apidoc.module.gulp-bundle-assets.using)

#### <a name="apidoc.element.gulp-bundle-assets.using.bundle"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.using.</span>bundle (key, type, env, bundleAllEnvironments)](#apidoc.element.gulp-bundle-assets.using.bundle)
- description and source-code
```javascript
bundle = function (key, type, env, bundleAllEnvironments) {
  var bundleName = this.bundleName(key, type, env, bundleAllEnvironments);
  var prefix = "Bundle '" + gutil.colors.green(bundleName) + "' using";
  return through.obj(function (file, enc, cb) {
    logger.log(prefix, gutil.colors.magenta(file.relative));
    this.push(file);
    cb();
  });
}
```
- example usage
```shell
...
module.exports.scripts = function (opts) {
var self = this,
  concatOpts = defaults({
    path: opts.bundleName + ((opts.isBundleAll && opts.env) ? '.' + opts.env : '') + '.js'
  }, opts.bundleOptions.pluginOptions['gulp-concat']);

return gulp.src(opts.src, {base: opts.base})
  .pipe(using.bundle(opts.bundleName, BundleKeys.SCRIPTS, opts.env, opts.isBundleAll))
  .pipe(through.obj(function (file, enc, cb) {
    self.attachStreamOptions(file, opts);
    this.push(file);
    cb();
  }))
  .pipe(gif(function (file) {
      return sourcemaps.isEnabled(opts);
...
```

#### <a name="apidoc.element.gulp-bundle-assets.using.bundleName"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.using.</span>bundleName (key, type, env, bundleAllEnvironments)](#apidoc.element.gulp-bundle-assets.using.bundleName)
- description and source-code
```javascript
bundleName = function (key, type, env, bundleAllEnvironments) {
  var envPrefix = '';
  if (bundleAllEnvironments) {
    envPrefix = env ? env + '.' : 'default.';
  }
  return envPrefix + key + '.' + type;
}
```
- example usage
```shell
...
      if (type === BundleKeys.SCRIPTS) {

        scriptWatch = namedBundleObj[BundleKeys.OPTIONS].watch[BundleKeys.SCRIPTS];

        if (scriptWatch !== false) {

          scriptsPath = pathifySrc(namedBundleObj[BundleKeys.SCRIPTS], base, namedBundleObj[BundleKeys.OPTIONS], env);
          prettyScriptsBundleName = using.bundleName(bundleName, BundleKeys.SCRIPTS, env, isBundleAll);

          logger.log("Starting '" + gutil.colors.cyan("watch") + "' for bundle '" + gutil.colors.green(prettyScriptsBundleName) + "'...");

          gulp.watch((typeof scriptWatch === 'string' || util.isArray(scriptWatch)) ? scriptWatch : scriptsPath)
            .on('change', function (file) { // log changed file?

var start = process.hrtime();
...
```

#### <a name="apidoc.element.gulp-bundle-assets.using.copy"></a>[function <span class="apidocSignatureSpan">gulp-bundle-assets.using.</span>copy (base)](#apidoc.element.gulp-bundle-assets.using.copy)
- description and source-code
```javascript
copy = function (base) {
  return through.obj(function (file, enc, cb) {
    var pathReplace = (base === '.') ? file.cwd : base;
    if (!stringHelper.endsWith(pathReplace, '/')) {
      pathReplace += '/';
    }
    logger.log("Copy file", gutil.colors.magenta(file.path.replace(pathReplace, '')));
    this.push(file);
    cb();
  });
}
```
- example usage
```shell
...
/**
* @param {String} item
* @param base
* @returns {*}
*/
StreamCopy.prototype.getStringCopyStream = function (item, base) {
 return gulp.src(pathifySrc(item, base), { base: base })
   .pipe(using.copy(base));
};

/**
* @param {Object} item
* @param base
* @returns {*}
*/
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
