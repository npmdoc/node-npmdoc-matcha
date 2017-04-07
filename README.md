# api documentation for  [matcha (v0.7.0)](https://github.com/logicalparadox/matcha#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-matcha.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-matcha) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-matcha.svg)](https://travis-ci.org/npmdoc/node-npmdoc-matcha)
#### Benchmark your code.

[![NPM](https://nodei.co/npm/matcha.png?downloads=true)](https://www.npmjs.com/package/matcha)

[![apidoc](https://npmdoc.github.io/node-npmdoc-matcha/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-matcha_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-matcha/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-matcha/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-matcha/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jake Luer",
        "email": "jake@alogicalparadox.com"
    },
    "bin": {
        "matcha": "./bin/matcha",
        "_matcha": "./bin/_matcha"
    },
    "bugs": {
        "url": "https://github.com/logicalparadox/matcha/issues"
    },
    "dependencies": {
        "electron": "0.4.x",
        "v8-argv": "0.1.x"
    },
    "description": "Benchmark your code.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "13f805409b37be57032c8458643bf1523ba68dda",
        "tarball": "https://registry.npmjs.org/matcha/-/matcha-0.7.0.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "4942f303ced7abe86babbecea3b498fbd336b321",
    "homepage": "https://github.com/logicalparadox/matcha#readme",
    "keyword": [
        "benchmark",
        "bench",
        "performance"
    ],
    "main": "index",
    "maintainers": [
        {
            "name": "jakeluer",
            "email": "jake.luer@incatern.com"
        }
    ],
    "name": "matcha",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/logicalparadox/matcha.git"
    },
    "scripts": {},
    "version": "0.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module matcha](#apidoc.module.matcha)
1.  [function <span class="apidocSignatureSpan">matcha.</span>Bench (title, fn)](#apidoc.element.matcha.Bench)
1.  [function <span class="apidocSignatureSpan">matcha.</span>Runner (suite)](#apidoc.element.matcha.Runner)
1.  [function <span class="apidocSignatureSpan">matcha.</span>Suite (title)](#apidoc.element.matcha.Suite)
1.  object <span class="apidocSignatureSpan">matcha.</span>Bench.prototype
1.  object <span class="apidocSignatureSpan">matcha.</span>Runner.prototype
1.  object <span class="apidocSignatureSpan">matcha.</span>Suite.prototype
1.  object <span class="apidocSignatureSpan">matcha.</span>utils
1.  object <span class="apidocSignatureSpan">matcha.</span>utils.cursor
1.  string <span class="apidocSignatureSpan">matcha.</span>version

#### [module matcha.Bench](#apidoc.module.matcha.Bench)
1.  [function <span class="apidocSignatureSpan">matcha.</span>Bench (title, fn)](#apidoc.element.matcha.Bench.Bench)
1.  [function <span class="apidocSignatureSpan">matcha.Bench.</span>super_ ()](#apidoc.element.matcha.Bench.super_)

#### [module matcha.Bench.prototype](#apidoc.module.matcha.Bench.prototype)
1.  [function <span class="apidocSignatureSpan">matcha.Bench.prototype.</span>run (cb)](#apidoc.element.matcha.Bench.prototype.run)

#### [module matcha.Runner](#apidoc.module.matcha.Runner)
1.  [function <span class="apidocSignatureSpan">matcha.</span>Runner (suite)](#apidoc.element.matcha.Runner.Runner)
1.  [function <span class="apidocSignatureSpan">matcha.Runner.</span>super_ ()](#apidoc.element.matcha.Runner.super_)

#### [module matcha.Runner.prototype](#apidoc.module.matcha.Runner.prototype)
1.  [function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>run (cb)](#apidoc.element.matcha.Runner.prototype.run)
1.  [function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runAfter (done)](#apidoc.element.matcha.Runner.prototype.runAfter)
1.  [function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runBefore (done)](#apidoc.element.matcha.Runner.prototype.runBefore)
1.  [function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runBenches (cb)](#apidoc.element.matcha.Runner.prototype.runBenches)
1.  [function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runSuites (done)](#apidoc.element.matcha.Runner.prototype.runSuites)

#### [module matcha.Suite](#apidoc.module.matcha.Suite)
1.  [function <span class="apidocSignatureSpan">matcha.</span>Suite (title)](#apidoc.element.matcha.Suite.Suite)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.</span>create (parent, title)](#apidoc.element.matcha.Suite.create)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.</span>super_ ()](#apidoc.element.matcha.Suite.super_)

#### [module matcha.Suite.prototype](#apidoc.module.matcha.Suite.prototype)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addAfter (fn)](#apidoc.element.matcha.Suite.prototype.addAfter)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addBefore (fn)](#apidoc.element.matcha.Suite.prototype.addBefore)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addBench (bench)](#apidoc.element.matcha.Suite.prototype.addBench)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addSuite (suite)](#apidoc.element.matcha.Suite.prototype.addSuite)
1.  [function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>setOption (key, value)](#apidoc.element.matcha.Suite.prototype.setOption)

#### [module matcha.utils](#apidoc.module.matcha.utils)
1.  [function <span class="apidocSignatureSpan">matcha.utils.</span>color (str, color)](#apidoc.element.matcha.utils.color)
1.  [function <span class="apidocSignatureSpan">matcha.utils.</span>highlight (str, color)](#apidoc.element.matcha.utils.highlight)
1.  [function <span class="apidocSignatureSpan">matcha.utils.</span>humanize (n)](#apidoc.element.matcha.utils.humanize)
1.  [function <span class="apidocSignatureSpan">matcha.utils.</span>padAfter (str, width)](#apidoc.element.matcha.utils.padAfter)
1.  [function <span class="apidocSignatureSpan">matcha.utils.</span>padBefore (str, width)](#apidoc.element.matcha.utils.padBefore)
1.  [function <span class="apidocSignatureSpan">matcha.utils.</span>series (arr, delay, iterator, done)](#apidoc.element.matcha.utils.series)
1.  object <span class="apidocSignatureSpan">matcha.utils.</span>cursor

#### [module matcha.utils.cursor](#apidoc.module.matcha.utils.cursor)
1.  [function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>CR ()](#apidoc.element.matcha.utils.cursor.CR)
1.  [function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>beginningOfLine ()](#apidoc.element.matcha.utils.cursor.beginningOfLine)
1.  [function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>deleteLine ()](#apidoc.element.matcha.utils.cursor.deleteLine)
1.  [function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>hide ()](#apidoc.element.matcha.utils.cursor.hide)
1.  [function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>show ()](#apidoc.element.matcha.utils.cursor.show)



# <a name="apidoc.module.matcha"></a>[module matcha](#apidoc.module.matcha)

#### <a name="apidoc.element.matcha.Bench"></a>[function <span class="apidocSignatureSpan">matcha.</span>Bench (title, fn)](#apidoc.element.matcha.Bench)
- description and source-code
```javascript
function Bench(title, fn) {
  EventEmitter.call(this);
  this.title = title;
  this.fn = fn;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Runner"></a>[function <span class="apidocSignatureSpan">matcha.</span>Runner (suite)](#apidoc.element.matcha.Runner)
- description and source-code
```javascript
function Runner(suite) {
  this.suite = suite;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite"></a>[function <span class="apidocSignatureSpan">matcha.</span>Suite (title)](#apidoc.element.matcha.Suite)
- description and source-code
```javascript
function Suite(title) {
  this.title = title || '';
  this.benches = [];
  this.suites = [];
  this.before = [];
  this.after = [];
  this.options = {
      type: 'adaptive'
    , iterations: 100
    , concurrency: 1
    , mintime: 500
    , delay: 100
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.Bench"></a>[module matcha.Bench](#apidoc.module.matcha.Bench)

#### <a name="apidoc.element.matcha.Bench.Bench"></a>[function <span class="apidocSignatureSpan">matcha.</span>Bench (title, fn)](#apidoc.element.matcha.Bench.Bench)
- description and source-code
```javascript
function Bench(title, fn) {
  EventEmitter.call(this);
  this.title = title;
  this.fn = fn;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Bench.super_"></a>[function <span class="apidocSignatureSpan">matcha.Bench.</span>super_ ()](#apidoc.element.matcha.Bench.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.Bench.prototype"></a>[module matcha.Bench.prototype](#apidoc.module.matcha.Bench.prototype)

#### <a name="apidoc.element.matcha.Bench.prototype.run"></a>[function <span class="apidocSignatureSpan">matcha.Bench.prototype.</span>run (cb)](#apidoc.element.matcha.Bench.prototype.run)
- description and source-code
```javascript
run = function (cb) {
  var self = this
    , opts = this.parent.options
    , runner = opts.type === 'static'
      ? runStatic
      : runAdaptive

  cb = cb || function () {};

  function report (total, elapsed) {
    var stats = {
        iterations: total
      , elapsed: elapsed
      , title: self.title
      , ops: Math.round(total / elapsed * 1000)
    };
    self.stats = stats;
    self.emit('end', stats);
    cb(stats);
  }

  runner.call(this, report);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.Runner"></a>[module matcha.Runner](#apidoc.module.matcha.Runner)

#### <a name="apidoc.element.matcha.Runner.Runner"></a>[function <span class="apidocSignatureSpan">matcha.</span>Runner (suite)](#apidoc.element.matcha.Runner.Runner)
- description and source-code
```javascript
function Runner(suite) {
  this.suite = suite;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Runner.super_"></a>[function <span class="apidocSignatureSpan">matcha.Runner.</span>super_ ()](#apidoc.element.matcha.Runner.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.Runner.prototype"></a>[module matcha.Runner.prototype](#apidoc.module.matcha.Runner.prototype)

#### <a name="apidoc.element.matcha.Runner.prototype.run"></a>[function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>run (cb)](#apidoc.element.matcha.Runner.prototype.run)
- description and source-code
```javascript
run = function (cb) {
  var self = this;

  var stats = this.stats = { suites: 0, benches: 0 };


  function iterator (fn, next) {
    fn(next);
  }

  this.on('bench start', function() {
    stats.benches++;
  });

  function done (err) {
    if (err) throw err;
    stats.elapsed = self.timer.stop().elapsed;
    self.emit('end', stats);
    cb()
  }

  this.timer = new Timer().start();
  this.emit('start');

  series([
      this.runBefore.bind(this)
    , this.runBenches.bind(this)
    , this.runSuites.bind(this)
    , this.runAfter.bind(this)
  ], iterator, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Runner.prototype.runAfter"></a>[function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runAfter (done)](#apidoc.element.matcha.Runner.prototype.runAfter)
- description and source-code
```javascript
runAfter = function (done) {
  runHooks.call(this, this.suite.after, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Runner.prototype.runBefore"></a>[function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runBefore (done)](#apidoc.element.matcha.Runner.prototype.runBefore)
- description and source-code
```javascript
runBefore = function (done) {
  runHooks.call(this, this.suite.before, done);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Runner.prototype.runBenches"></a>[function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runBenches (cb)](#apidoc.element.matcha.Runner.prototype.runBenches)
- description and source-code
```javascript
runBenches = function (cb) {
  var self = this
    , suite = this.suite
    , stats = []
    , delay = suite.options.delay;

  series(suite.benches, delay, function (bench, next) {
    self.emit('bench start', bench);
    bench.run(function (res) {
      stats.push(res);
      self.emit('bench end', res);
      next();
    });
  }, function () {
    self.emit('suite results', stats);
    cb();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Runner.prototype.runSuites"></a>[function <span class="apidocSignatureSpan">matcha.Runner.prototype.</span>runSuites (done)](#apidoc.element.matcha.Runner.prototype.runSuites)
- description and source-code
```javascript
runSuites = function (done) {
  var self = this
    , suite = this.suite
    , delay = suite.options.delay;

  series(suite.suites, delay, function (suite, next) {
    var runner = new Runner(suite);
    proxy(runner, self, 'suite start');
    proxy(runner, self, 'suite end');
    proxy(runner, self, 'suite results');
    proxy(runner, self, 'bench start');
    proxy(runner, self, 'bench end');
    self.emit('suite start', suite);
    runner.run(function () {
      self.stats.suites++;
      self.emit('suite end', suite);
      next();
    });
  }, done);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.Suite"></a>[module matcha.Suite](#apidoc.module.matcha.Suite)

#### <a name="apidoc.element.matcha.Suite.Suite"></a>[function <span class="apidocSignatureSpan">matcha.</span>Suite (title)](#apidoc.element.matcha.Suite.Suite)
- description and source-code
```javascript
function Suite(title) {
  this.title = title || '';
  this.benches = [];
  this.suites = [];
  this.before = [];
  this.after = [];
  this.options = {
      type: 'adaptive'
    , iterations: 100
    , concurrency: 1
    , mintime: 500
    , delay: 100
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite.create"></a>[function <span class="apidocSignatureSpan">matcha.Suite.</span>create (parent, title)](#apidoc.element.matcha.Suite.create)
- description and source-code
```javascript
create = function (parent, title) {
  var suite = new Suite(title);
  parent.addSuite(suite);
  return suite;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite.super_"></a>[function <span class="apidocSignatureSpan">matcha.Suite.</span>super_ ()](#apidoc.element.matcha.Suite.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.Suite.prototype"></a>[module matcha.Suite.prototype](#apidoc.module.matcha.Suite.prototype)

#### <a name="apidoc.element.matcha.Suite.prototype.addAfter"></a>[function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addAfter (fn)](#apidoc.element.matcha.Suite.prototype.addAfter)
- description and source-code
```javascript
addAfter = function (fn) {
  this.after.push(fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite.prototype.addBefore"></a>[function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addBefore (fn)](#apidoc.element.matcha.Suite.prototype.addBefore)
- description and source-code
```javascript
addBefore = function (fn) {
  this.before.push(fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite.prototype.addBench"></a>[function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addBench (bench)](#apidoc.element.matcha.Suite.prototype.addBench)
- description and source-code
```javascript
addBench = function (bench) {
  bench.parent = this;
  this.benches.push(bench);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite.prototype.addSuite"></a>[function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>addSuite (suite)](#apidoc.element.matcha.Suite.prototype.addSuite)
- description and source-code
```javascript
addSuite = function (suite) {
  suite.parent = this;
  this.suites.push(suite);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.Suite.prototype.setOption"></a>[function <span class="apidocSignatureSpan">matcha.Suite.prototype.</span>setOption (key, value)](#apidoc.element.matcha.Suite.prototype.setOption)
- description and source-code
```javascript
setOption = function (key, value) {
  this.options[key] = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.utils"></a>[module matcha.utils](#apidoc.module.matcha.utils)

#### <a name="apidoc.element.matcha.utils.color"></a>[function <span class="apidocSignatureSpan">matcha.utils.</span>color (str, color)](#apidoc.element.matcha.utils.color)
- description and source-code
```javascript
color = function (str, color) {
  var options = {
      red:      '\u001b[31m'
    , green:    '\u001b[32m'
    , yellow:   '\u001b[33m'
    , blue:     '\u001b[34m'
    , magenta:  '\u001b[35m'
    , cyan:     '\u001b[36m'
    , gray:     '\u001b[90m'
    , reset:    '\u001b[0m'
  };
  return options[color] + str + options.reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.highlight"></a>[function <span class="apidocSignatureSpan">matcha.utils.</span>highlight (str, color)](#apidoc.element.matcha.utils.highlight)
- description and source-code
```javascript
highlight = function (str, color) {
  var options = {
      red:      '\u001b[41m'
    , green:    '\u001b[42m'
    , yellow:   '\u001b[43m'
    , blue:     '\u001b[44m'
    , magenta:  '\u001b[45m'
    , cyan:     '\u001b[46m'
    , gray:     '\u001b[100m'
    , reset:    '\u001b[0m'
  };
  return options[color] + str + options.reset;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.humanize"></a>[function <span class="apidocSignatureSpan">matcha.utils.</span>humanize (n)](#apidoc.element.matcha.utils.humanize)
- description and source-code
```javascript
humanize = function (n) {
  var n = String(n).split('.')
  n[0] = n[0].replace(/(\d)(?=(\d\d\d)+(?!\d))/g, '$1,');
  return n.join('.')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.padAfter"></a>[function <span class="apidocSignatureSpan">matcha.utils.</span>padAfter (str, width)](#apidoc.element.matcha.utils.padAfter)
- description and source-code
```javascript
padAfter = function (str, width) {
  return str + Array(width - str.length).join(' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.padBefore"></a>[function <span class="apidocSignatureSpan">matcha.utils.</span>padBefore (str, width)](#apidoc.element.matcha.utils.padBefore)
- description and source-code
```javascript
padBefore = function (str, width) {
  return Array(width - str.length).join(' ') + str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.series"></a>[function <span class="apidocSignatureSpan">matcha.utils.</span>series (arr, delay, iterator, done)](#apidoc.element.matcha.utils.series)
- description and source-code
```javascript
series = function (arr, delay, iterator, done) {
  if ('function' == typeof delay) {
    done = iterator;
    iterator = delay;
    delay = 0;
  }

  done = done || function () {};

  function iterate (i) {
    var fn = arr[i];
    if (!fn) return done();
    iterator(fn, function cb(err) {
      if (err) return done(err);
      if (!delay) return iterate(++i);
      setTimeout(function () {
        iterate(++i);
      }, delay);
    });
  };

  iterate(0);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.matcha.utils.cursor"></a>[module matcha.utils.cursor](#apidoc.module.matcha.utils.cursor)

#### <a name="apidoc.element.matcha.utils.cursor.CR"></a>[function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>CR ()](#apidoc.element.matcha.utils.cursor.CR)
- description and source-code
```javascript
CR = function () {
  exports.cursor.deleteLine();
  exports.cursor.beginningOfLine();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.cursor.beginningOfLine"></a>[function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>beginningOfLine ()](#apidoc.element.matcha.utils.cursor.beginningOfLine)
- description and source-code
```javascript
beginningOfLine = function () {
  process.stdout.write('\033[0G');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.cursor.deleteLine"></a>[function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>deleteLine ()](#apidoc.element.matcha.utils.cursor.deleteLine)
- description and source-code
```javascript
deleteLine = function () {
  process.stdout.write('\033[2K');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.cursor.hide"></a>[function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>hide ()](#apidoc.element.matcha.utils.cursor.hide)
- description and source-code
```javascript
hide = function () {
  process.stdout.write('\033[?25l');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.matcha.utils.cursor.show"></a>[function <span class="apidocSignatureSpan">matcha.utils.cursor.</span>show ()](#apidoc.element.matcha.utils.cursor.show)
- description and source-code
```javascript
show = function () {
  process.stdout.write('\033[?25h');
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
