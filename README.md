# api documentation for  [nodeunit (v0.11.0)](https://github.com/caolan/nodeunit#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nodeunit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nodeunit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nodeunit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nodeunit)
#### Easy unit testing for node.js and the browser.

[![NPM](https://nodei.co/npm/nodeunit.png?downloads=true)](https://www.npmjs.com/package/nodeunit)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nodeunit/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nodeunit_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nodeunit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nodeunit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nodeunit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "nodeunit": "./bin/nodeunit"
    },
    "bugs": {
        "url": "http://github.com/caolan/nodeunit/issues"
    },
    "contributors": [
        {
            "name": "Romain Beauxis",
            "url": "https://github.com/toots"
        },
        {
            "name": "Alex Gorbatchev",
            "url": "https://github.com/alexgorbatchev"
        },
        {
            "name": "Alex Wolfe",
            "url": "https://github.com/alexkwolfe"
        },
        {
            "name": "Carl Fürstenberg",
            "url": "https://github.com/azatoth"
        },
        {
            "name": "Gerad Suyderhoud",
            "url": "https://github.com/gerad"
        },
        {
            "name": "Kadir Pekel",
            "url": "https://github.com/coffeemate"
        },
        {
            "name": "Oleg Efimov",
            "url": "https://github.com/Sannis"
        },
        {
            "name": "Orlando Vazquez",
            "url": "https://github.com/orlandov"
        },
        {
            "name": "Ryan Dahl",
            "url": "https://github.com/ry"
        },
        {
            "name": "Sam Stephenson",
            "url": "https://github.com/sstephenson"
        },
        {
            "name": "Thomas Mayfield",
            "url": "https://github.com/thegreatape"
        },
        {
            "name": "Elijah Insua",
            "email": "tmpvar@gmail.com",
            "url": "http://tmpvar.com"
        }
    ],
    "dependencies": {
        "ejs": "^2.5.2",
        "tap": "^10.0.2"
    },
    "description": "Easy unit testing for node.js and the browser.",
    "devDependencies": {
        "should": ">=11.1.0",
        "uglify-js": ">=2.7.3"
    },
    "directories": {
        "lib": "./lib",
        "doc": "./doc",
        "man": "./man1"
    },
    "dist": {
        "shasum": "5f57579e2a7f3286fd04937bfd5665070c4e015c",
        "tarball": "https://registry.npmjs.org/nodeunit/-/nodeunit-0.11.0.tgz"
    },
    "gitHead": "be1bde2e095c2c08de3255368997279dc6eb7872",
    "homepage": "https://github.com/caolan/nodeunit#readme",
    "license": "MIT",
    "maintainers": [
        {
            "name": "caolan",
            "email": "caolan@caolanmcmahon.com"
        },
        {
            "name": "mreinstein",
            "email": "reinstein.mike@gmail.com"
        }
    ],
    "man": [
        "/Users/michaelreinstein/wwwroot/nodeunit/man1/nodeunit.1"
    ],
    "name": "nodeunit",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/caolan/nodeunit.git"
    },
    "scripts": {
        "test": "node ./bin/nodeunit"
    },
    "version": "0.11.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nodeunit](#apidoc.module.nodeunit)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>addListener (type, listener)](#apidoc.element.nodeunit.addListener)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>assert.AssertionError {{signature}}](#apidoc.element.nodeunit.assert.AssertionError)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>complete (name, assertions)](#apidoc.element.nodeunit.complete)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>done ()](#apidoc.element.nodeunit.done)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>emit (type)](#apidoc.element.nodeunit.emit)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>eventNames ()](#apidoc.element.nodeunit.eventNames)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>getMaxListeners ()](#apidoc.element.nodeunit.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>listenerCount (type)](#apidoc.element.nodeunit.listenerCount)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>listeners (type)](#apidoc.element.nodeunit.listeners)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>on (type, listener)](#apidoc.element.nodeunit.on)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>once (type, listener)](#apidoc.element.nodeunit.once)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>prependListener (type, listener)](#apidoc.element.nodeunit.prependListener)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>prependOnceListener (type, listener)](#apidoc.element.nodeunit.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>removeAllListeners (type)](#apidoc.element.nodeunit.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>removeListener (type, listener)](#apidoc.element.nodeunit.removeListener)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>runFiles (paths, opt)](#apidoc.element.nodeunit.runFiles)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>runModule (name, mod, opt, callback)](#apidoc.element.nodeunit.runModule)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>runModules (modules, opt)](#apidoc.element.nodeunit.runModules)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>runSuite (name, suite, opt, callback)](#apidoc.element.nodeunit.runSuite)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>runTest (name, fn, opt, callback)](#apidoc.element.nodeunit.runTest)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>setMaxListeners (n)](#apidoc.element.nodeunit.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">nodeunit.</span>testCase (suite)](#apidoc.element.nodeunit.testCase)
1.  object <span class="apidocSignatureSpan">nodeunit.</span>assert
1.  object <span class="apidocSignatureSpan">nodeunit.</span>assert.AssertionError.prototype
1.  object <span class="apidocSignatureSpan">nodeunit.</span>async
1.  object <span class="apidocSignatureSpan">nodeunit.</span>core
1.  object <span class="apidocSignatureSpan">nodeunit.</span>reporters
1.  object <span class="apidocSignatureSpan">nodeunit.</span>testrunner
1.  object <span class="apidocSignatureSpan">nodeunit.</span>track
1.  object <span class="apidocSignatureSpan">nodeunit.</span>types
1.  object <span class="apidocSignatureSpan">nodeunit.</span>utils

#### [module nodeunit.assert](#apidoc.module.nodeunit.assert)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>AssertionError {{signature}}](#apidoc.element.nodeunit.assert.AssertionError)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>deepEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.deepEqual)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>doesNotThrow (block, error, message)](#apidoc.element.nodeunit.assert.doesNotThrow)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>equal (actual, expected, message)](#apidoc.element.nodeunit.assert.equal)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>fail (actual, expected, message, operator, stackStartFunction)](#apidoc.element.nodeunit.assert.fail)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>ifError (err)](#apidoc.element.nodeunit.assert.ifError)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>notDeepEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.notDeepEqual)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>notEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.notEqual)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>notStrictEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.notStrictEqual)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>ok (value, message)](#apidoc.element.nodeunit.assert.ok)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>strictEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.strictEqual)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>throws (block, error, message)](#apidoc.element.nodeunit.assert.throws)

#### [module nodeunit.assert.AssertionError](#apidoc.module.nodeunit.assert.AssertionError)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.</span>AssertionError {{signature}}](#apidoc.element.nodeunit.assert.AssertionError.AssertionError)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.AssertionError.</span>super_ ()](#apidoc.element.nodeunit.assert.AssertionError.super_)

#### [module nodeunit.assert.AssertionError.prototype](#apidoc.module.nodeunit.assert.AssertionError.prototype)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.AssertionError.prototype.</span>constructor {{signature}}](#apidoc.element.nodeunit.assert.AssertionError.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nodeunit.assert.AssertionError.prototype.</span>toString ()](#apidoc.element.nodeunit.assert.AssertionError.prototype.toString)

#### [module nodeunit.async](#apidoc.module.nodeunit.async)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>all (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.all)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>any (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.any)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>apply (fn)](#apidoc.element.nodeunit.async.apply)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>auto (tasks, callback)](#apidoc.element.nodeunit.async.auto)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>concat ()](#apidoc.element.nodeunit.async.concat)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>concatSeries ()](#apidoc.element.nodeunit.async.concatSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>detect ()](#apidoc.element.nodeunit.async.detect)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>detectSeries ()](#apidoc.element.nodeunit.async.detectSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>dir (fn)](#apidoc.element.nodeunit.async.dir)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>every (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.every)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>filter ()](#apidoc.element.nodeunit.async.filter)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>filterSeries ()](#apidoc.element.nodeunit.async.filterSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>foldl (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.foldl)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>foldr (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.foldr)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>forEach (arr, iterator, callback)](#apidoc.element.nodeunit.async.forEach)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>forEachSeries (arr, iterator, callback)](#apidoc.element.nodeunit.async.forEachSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>inject (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.inject)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>iterator (tasks)](#apidoc.element.nodeunit.async.iterator)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>log (fn)](#apidoc.element.nodeunit.async.log)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>map ()](#apidoc.element.nodeunit.async.map)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>mapSeries ()](#apidoc.element.nodeunit.async.mapSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>memoize (fn, hasher)](#apidoc.element.nodeunit.async.memoize)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>nextTick (fn)](#apidoc.element.nodeunit.async.nextTick)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>noConflict ()](#apidoc.element.nodeunit.async.noConflict)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>parallel (tasks, callback)](#apidoc.element.nodeunit.async.parallel)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>queue (worker, concurrency)](#apidoc.element.nodeunit.async.queue)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>reduce (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.reduce)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>reduceRight (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.reduceRight)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>reject ()](#apidoc.element.nodeunit.async.reject)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>rejectSeries ()](#apidoc.element.nodeunit.async.rejectSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>select ()](#apidoc.element.nodeunit.async.select)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>selectSeries ()](#apidoc.element.nodeunit.async.selectSeries)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>series (tasks, callback)](#apidoc.element.nodeunit.async.series)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>some (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.some)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>sortBy (arr, iterator, callback)](#apidoc.element.nodeunit.async.sortBy)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>until (test, iterator, callback)](#apidoc.element.nodeunit.async.until)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>waterfall (tasks, callback)](#apidoc.element.nodeunit.async.waterfall)
1.  [function <span class="apidocSignatureSpan">nodeunit.async.</span>whilst (test, iterator, callback)](#apidoc.element.nodeunit.async.whilst)

#### [module nodeunit.core](#apidoc.module.nodeunit.core)
1.  [function <span class="apidocSignatureSpan">nodeunit.core.</span>runModule (name, mod, opt, callback)](#apidoc.element.nodeunit.core.runModule)
1.  [function <span class="apidocSignatureSpan">nodeunit.core.</span>runModules (modules, opt)](#apidoc.element.nodeunit.core.runModules)
1.  [function <span class="apidocSignatureSpan">nodeunit.core.</span>runSuite (name, suite, opt, callback)](#apidoc.element.nodeunit.core.runSuite)
1.  [function <span class="apidocSignatureSpan">nodeunit.core.</span>runTest (name, fn, opt, callback)](#apidoc.element.nodeunit.core.runTest)
1.  [function <span class="apidocSignatureSpan">nodeunit.core.</span>testCase (suite)](#apidoc.element.nodeunit.core.testCase)

#### [module nodeunit.testrunner](#apidoc.module.nodeunit.testrunner)
1.  [function <span class="apidocSignatureSpan">nodeunit.testrunner.</span>run ()](#apidoc.element.nodeunit.testrunner.run)

#### [module nodeunit.track](#apidoc.module.nodeunit.track)
1.  [function <span class="apidocSignatureSpan">nodeunit.track.</span>createTracker (on_exit)](#apidoc.element.nodeunit.track.createTracker)
1.  [function <span class="apidocSignatureSpan">nodeunit.track.</span>default_on_exit (tracker)](#apidoc.element.nodeunit.track.default_on_exit)

#### [module nodeunit.types](#apidoc.module.nodeunit.types)
1.  [function <span class="apidocSignatureSpan">nodeunit.types.</span>assertion (obj)](#apidoc.element.nodeunit.types.assertion)
1.  [function <span class="apidocSignatureSpan">nodeunit.types.</span>assertionList (arr, duration)](#apidoc.element.nodeunit.types.assertionList)
1.  [function <span class="apidocSignatureSpan">nodeunit.types.</span>options (opt)](#apidoc.element.nodeunit.types.options)
1.  [function <span class="apidocSignatureSpan">nodeunit.types.</span>test (name, start, options, callback)](#apidoc.element.nodeunit.types.test)

#### [module nodeunit.utils](#apidoc.module.nodeunit.utils)
1.  [function <span class="apidocSignatureSpan">nodeunit.utils.</span>betterErrors (assertion)](#apidoc.element.nodeunit.utils.betterErrors)
1.  [function <span class="apidocSignatureSpan">nodeunit.utils.</span>httputil (cgi, envReady)](#apidoc.element.nodeunit.utils.httputil)
1.  [function <span class="apidocSignatureSpan">nodeunit.utils.</span>modulePaths (paths, callback, recursive)](#apidoc.element.nodeunit.utils.modulePaths)
1.  [function <span class="apidocSignatureSpan">nodeunit.utils.</span>sandbox (files, sandbox)](#apidoc.element.nodeunit.utils.sandbox)



# <a name="apidoc.module.nodeunit"></a>[module nodeunit](#apidoc.module.nodeunit)

#### <a name="apidoc.element.nodeunit.addListener"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>addListener (type, listener)](#apidoc.element.nodeunit.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.AssertionError"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>assert.AssertionError {{signature}}](#apidoc.element.nodeunit.assert.AssertionError)
- description and source-code
```javascript
AssertionError
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.complete"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>complete (name, assertions)](#apidoc.element.nodeunit.complete)
- description and source-code
```javascript
complete = function (name, assertions)
{
    exports.emit('complete', name, assertions);
}
```
- example usage
```shell
...
   var start = new Date().getTime();

   exports.runSuite(null, mod, options, function (err, a_list) {
       var end = new Date().getTime();
       var assertion_list = types.assertionList(a_list, end - start);
       options.moduleDone(name, assertion_list);
       if (nodeunit.complete) {
           nodeunit.complete(name, assertion_list);
       }
       callback(null, a_list);
   });
};

/**
* Treats an object literal as a list of modules keyed by name. Runs each
...
```

#### <a name="apidoc.element.nodeunit.done"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>done ()](#apidoc.element.nodeunit.done)
- description and source-code
```javascript
done = function ()
{
    exports.emit('done');
}
```
- example usage
```shell
...
-----

Here is an example unit test module:

exports.testSomething = function(test) {
    test.expect(1);
    test.ok(true, "this assertion should pass");
    test.done();
};

exports.testSomethingElse = function(test) {
    test.ok(false, "this assertion should fail");
    test.done();
};
...
```

#### <a name="apidoc.element.nodeunit.emit"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>emit (type)](#apidoc.element.nodeunit.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.eventNames"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>eventNames ()](#apidoc.element.nodeunit.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.getMaxListeners"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>getMaxListeners ()](#apidoc.element.nodeunit.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.listenerCount"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>listenerCount (type)](#apidoc.element.nodeunit.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.listeners"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>listeners (type)](#apidoc.element.nodeunit.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.on"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>on (type, listener)](#apidoc.element.nodeunit.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
            names[testname] = testname;
        },
        remove: function (testname) {
            delete names[testname];
        }
    };

    process.on('exit', function() {
        on_exit = on_exit || exports.default_on_exit;
        on_exit(tracker);
    });

    return tracker;
};
...
```

#### <a name="apidoc.element.nodeunit.once"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>once (type, listener)](#apidoc.element.nodeunit.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.prependListener"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>prependListener (type, listener)](#apidoc.element.nodeunit.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.prependOnceListener"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>prependOnceListener (type, listener)](#apidoc.element.nodeunit.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.removeAllListeners"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>removeAllListeners (type)](#apidoc.element.nodeunit.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.removeListener"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>removeListener (type, listener)](#apidoc.element.nodeunit.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.runFiles"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>runFiles (paths, opt)](#apidoc.element.nodeunit.runFiles)
- description and source-code
```javascript
runFiles = function (paths, opt) {
    var all_assertions = [];
    var options = types.options(opt);
    var start = new Date().getTime();

    if (!paths.length) {
        return options.done(types.assertionList(all_assertions));
    }

    utils.modulePaths(paths, function (err, files) {
        if (err) throw err;
        async.concatSeries(files, function (file, cb) {
            var name = path.basename(file);
            exports.runModule(name, require(file), options, cb);
        },
        function (err, all_assertions) {
            var end = new Date().getTime();
            exports.done()
            options.done(types.assertionList(all_assertions, end - start));
        });
    }, options.recursive);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.runModule"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>runModule (name, mod, opt, callback)](#apidoc.element.nodeunit.runModule)
- description and source-code
```javascript
runModule = function (name, mod, opt, callback) {
    var options = _copy(types.options(opt));

    var _run = false;
    var _moduleStart = options.moduleStart;

    mod = wrapGroup(mod);

    function run_once() {
        if (!_run) {
            _run = true;
            _moduleStart(name);
        }
    }
    options.moduleStart = run_once;

    var start = new Date().getTime();

    exports.runSuite(null, mod, options, function (err, a_list) {
        var end = new Date().getTime();
        var assertion_list = types.assertionList(a_list, end - start);
        options.moduleDone(name, assertion_list);
        if (nodeunit.complete) {
            nodeunit.complete(name, assertion_list);
        }
        callback(null, a_list);
    });
}
```
- example usage
```shell
...
// TODO: add proper unit tests for this function
exports.runModules = function (modules, opt) {
    var all_assertions = [];
    var options = types.options(opt);
    var start = new Date().getTime();

    async.concatSeries(_keys(modules), function (k, cb) {
        exports.runModule(k, modules[k], options, cb);
    },
    function (err, all_assertions) {
        var end = new Date().getTime();
        options.done(types.assertionList(all_assertions, end - start));
    });
};
...
```

#### <a name="apidoc.element.nodeunit.runModules"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>runModules (modules, opt)](#apidoc.element.nodeunit.runModules)
- description and source-code
```javascript
runModules = function (modules, opt) {
    var all_assertions = [];
    var options = types.options(opt);
    var start = new Date().getTime();

    async.concatSeries(_keys(modules), function (k, cb) {
        exports.runModule(k, modules[k], options, cb);
    },
    function (err, all_assertions) {
        var end = new Date().getTime();
        options.done(types.assertionList(all_assertions, end - start));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.runSuite"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>runSuite (name, suite, opt, callback)](#apidoc.element.nodeunit.runSuite)
- description and source-code
```javascript
runSuite = function (name, suite, opt, callback) {
    suite = wrapGroup(suite);
    var keys = _keys(suite);

    async.concatSeries(keys, function (k, cb) {
        var prop = suite[k], _name;

        _name = name ? [].concat(name, k) : [k];
        _name.toString = function () {
            // fallback for old one
            return this.join(' - ');
        };

        if (typeof prop === 'function') {
            var in_name = false,
                in_specific_test = (_name.toString() === opt.testFullSpec) ? true : false;
            for (var i = 0; i < _name.length; i += 1) {
                if (_name[i] === opt.testspec) {
                    in_name = true;
                }
            }

            if ((!opt.testFullSpec || in_specific_test) && (!opt.testspec || in_name)) {
                if (opt.moduleStart) {
                    opt.moduleStart();
                }
                exports.runTest(_name, suite[k], opt, cb);
            }
            else {
                return cb();
            }
        }
        else {
            exports.runSuite(_name, suite[k], opt, cb);
        }
    }, callback);
}
```
- example usage
```shell
...
               exports.runTest(_name, suite[k], opt, cb);
           }
           else {
               return cb();
           }
       }
       else {
           exports.runSuite(_name, suite[k], opt, cb);
       }
   }, callback);
};

/**
* Run each exported test function or test suite from a loaded module.
*
...
```

#### <a name="apidoc.element.nodeunit.runTest"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>runTest (name, fn, opt, callback)](#apidoc.element.nodeunit.runTest)
- description and source-code
```javascript
runTest = function (name, fn, opt, callback) {
    var options = types.options(opt);

    options.testStart(name);
    var start = new Date().getTime();
    var test = types.test(name, start, options, callback);

    options.testReady(test);
    try {
        fn(test);
    }
    catch (e) {
        test.done(e);
    }
}
```
- example usage
```shell
...
        }
    }

    if ((!opt.testFullSpec || in_specific_test) && (!opt.testspec || in_name)) {
        if (opt.moduleStart) {
            opt.moduleStart();
        }
        exports.runTest(_name, suite[k], opt, cb);
    }
    else {
        return cb();
    }
}
else {
    exports.runSuite(_name, suite[k], opt, cb);
...
```

#### <a name="apidoc.element.nodeunit.setMaxListeners"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>setMaxListeners (n)](#apidoc.element.nodeunit.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.testCase"></a>[function <span class="apidocSignatureSpan">nodeunit.</span>testCase (suite)](#apidoc.element.nodeunit.testCase)
- description and source-code
```javascript
testCase = function (suite) {
    return suite;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodeunit.assert"></a>[module nodeunit.assert](#apidoc.module.nodeunit.assert)

#### <a name="apidoc.element.nodeunit.assert.AssertionError"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>AssertionError {{signature}}](#apidoc.element.nodeunit.assert.AssertionError)
- description and source-code
```javascript
AssertionError
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.deepEqual"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>deepEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.deepEqual)
- description and source-code
```javascript
function deepEqual(actual, expected, message) {
  if (!_deepEqual(actual, expected)) {
    fail(actual, expected, message, "deepEqual", assert.deepEqual);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.doesNotThrow"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>doesNotThrow (block, error, message)](#apidoc.element.nodeunit.assert.doesNotThrow)
- description and source-code
```javascript
doesNotThrow = function (block, error, message) {
  _throws.apply(this, [false].concat(pSlice.call(arguments)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.equal"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>equal (actual, expected, message)](#apidoc.element.nodeunit.assert.equal)
- description and source-code
```javascript
function equal(actual, expected, message) {
  if (actual != expected) fail(actual, expected, message, "==", assert.equal);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.fail"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>fail (actual, expected, message, operator, stackStartFunction)](#apidoc.element.nodeunit.assert.fail)
- description and source-code
```javascript
function fail(actual, expected, message, operator, stackStartFunction) {
  throw new assert.AssertionError({
    message: message,
    actual: actual,
    expected: expected,
    operator: operator,
    stackStartFunction: stackStartFunction
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.ifError"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>ifError (err)](#apidoc.element.nodeunit.assert.ifError)
- description and source-code
```javascript
ifError = function (err) { if (err) {throw err;}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.notDeepEqual"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>notDeepEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.notDeepEqual)
- description and source-code
```javascript
function notDeepEqual(actual, expected, message) {
  if (_deepEqual(actual, expected)) {
    fail(actual, expected, message, "notDeepEqual", assert.notDeepEqual);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.notEqual"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>notEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.notEqual)
- description and source-code
```javascript
function notEqual(actual, expected, message) {
  if (actual == expected) {
    fail(actual, expected, message, "!=", assert.notEqual);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.notStrictEqual"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>notStrictEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.notStrictEqual)
- description and source-code
```javascript
function notStrictEqual(actual, expected, message) {
  if (actual === expected) {
    fail(actual, expected, message, "!==", assert.notStrictEqual);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.ok"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>ok (value, message)](#apidoc.element.nodeunit.assert.ok)
- description and source-code
```javascript
function ok(value, message) {
  if (!!!value) fail(value, true, message, "==", assert.ok);
}
```
- example usage
```shell
...
Usage
-----

Here is an example unit test module:

exports.testSomething = function(test) {
    test.expect(1);
    test.ok(true, "this assertion should pass");
    test.done();
};

exports.testSomethingElse = function(test) {
    test.ok(false, "this assertion should fail");
    test.done();
};
...
```

#### <a name="apidoc.element.nodeunit.assert.strictEqual"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>strictEqual (actual, expected, message)](#apidoc.element.nodeunit.assert.strictEqual)
- description and source-code
```javascript
function strictEqual(actual, expected, message) {
  if (actual !== expected) {
    fail(actual, expected, message, "===", assert.strictEqual);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.throws"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>throws (block, error, message)](#apidoc.element.nodeunit.assert.throws)
- description and source-code
```javascript
throws = function (block, error, message) {
  _throws.apply(this, [true].concat(pSlice.call(arguments)));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodeunit.assert.AssertionError"></a>[module nodeunit.assert.AssertionError](#apidoc.module.nodeunit.assert.AssertionError)

#### <a name="apidoc.element.nodeunit.assert.AssertionError.AssertionError"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.</span>AssertionError {{signature}}](#apidoc.element.nodeunit.assert.AssertionError.AssertionError)
- description and source-code
```javascript
AssertionError
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.AssertionError.super_"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.AssertionError.</span>super_ ()](#apidoc.element.nodeunit.assert.AssertionError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodeunit.assert.AssertionError.prototype"></a>[module nodeunit.assert.AssertionError.prototype](#apidoc.module.nodeunit.assert.AssertionError.prototype)

#### <a name="apidoc.element.nodeunit.assert.AssertionError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.AssertionError.prototype.</span>constructor {{signature}}](#apidoc.element.nodeunit.assert.AssertionError.prototype.constructor)
- description and source-code
```javascript
AssertionError
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.assert.AssertionError.prototype.toString"></a>[function <span class="apidocSignatureSpan">nodeunit.assert.AssertionError.prototype.</span>toString ()](#apidoc.element.nodeunit.assert.AssertionError.prototype.toString)
- description and source-code
```javascript
toString = function () {
  if (this.message) {
    return [this.name+":", this.message].join(' ');
  } else {
    return [ this.name+":"
           , typeof this.expected !== 'undefined' ? JSON.stringify(this.expected) : 'undefined'
           , this.operator
           , typeof this.actual !== 'undefined' ? JSON.stringify(this.actual) : 'undefined'
           ].join(" ");
  }
}
```
- example usage
```shell
...
// sequences.

    escapable.lastIndex = 0;
    return escapable.test(string) ?
        '"' + string.replace(escapable, function (a) {
            var c = meta[a];
            return typeof c === 'string' ? c :
                '\\u' + ('0000' + a.charCodeAt(0).toString(16)).slice(-4);
        }) + '"' :
        '"' + string + '"';
}


function str(key, holder) {
...
```



# <a name="apidoc.module.nodeunit.async"></a>[module nodeunit.async](#apidoc.module.nodeunit.async)

#### <a name="apidoc.element.nodeunit.async.all"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>all (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.all)
- description and source-code
```javascript
all = function (arr, iterator, main_callback) {
    async.forEach(arr, function (x, callback) {
        iterator(x, function (v) {
            if (!v) {
                main_callback(false);
                main_callback = function () {};
            }
            callback();
        });
    }, function (err) {
        main_callback(true);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.any"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>any (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.any)
- description and source-code
```javascript
any = function (arr, iterator, main_callback) {
    async.forEach(arr, function (x, callback) {
        iterator(x, function (v) {
            if (v) {
                main_callback(true);
                main_callback = function () {};
            }
            callback();
        });
    }, function (err) {
        main_callback(false);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.apply"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>apply (fn)](#apidoc.element.nodeunit.async.apply)
- description and source-code
```javascript
apply = function (fn) {
    var args = Array.prototype.slice.call(arguments, 1);
    return function () {
        return fn.apply(
            null, args.concat(Array.prototype.slice.call(arguments))
        );
    };
}
```
- example usage
```shell
...
    iterate();
};


var doParallel = function (fn) {
    return function () {
        var args = Array.prototype.slice.call(arguments);
        return fn.apply(null, [async.forEach].concat(args));
    };
};
var doSeries = function (fn) {
    return function () {
        var args = Array.prototype.slice.call(arguments);
        return fn.apply(null, [async.forEachSeries].concat(args));
    };
...
```

#### <a name="apidoc.element.nodeunit.async.auto"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>auto (tasks, callback)](#apidoc.element.nodeunit.async.auto)
- description and source-code
```javascript
auto = function (tasks, callback) {
    callback = callback || function () {};
    var keys = _keys(tasks);
    if (!keys.length) {
        return callback(null);
    }

    var completed = [];

    var listeners = [];
    var addListener = function (fn) {
        listeners.unshift(fn);
    };
    var removeListener = function (fn) {
        for (var i = 0; i < listeners.length; i += 1) {
            if (listeners[i] === fn) {
                listeners.splice(i, 1);
                return;
            }
        }
    };
    var taskComplete = function () {
        _forEach(listeners, function (fn) {
            fn();
        });
    };

    addListener(function () {
        if (completed.length === keys.length) {
            callback(null);
        }
    });

    _forEach(keys, function (k) {
        var task = (tasks[k] instanceof Function) ? [tasks[k]]: tasks[k];
        var taskCallback = function (err) {
            if (err) {
                callback(err);
                // stop subsequent errors hitting callback multiple times
                callback = function () {};
            }
            else {
                completed.push(k);
                taskComplete();
            }
        };
        var requires = task.slice(0, Math.abs(task.length - 1)) || [];
        var ready = function () {
            return _reduce(requires, function (a, x) {
                return (a && _indexOf(completed, x) !== -1);
            }, true);
        };
        if (ready()) {
            task[task.length - 1](taskCallback);
        }
        else {
            var listener = function () {
                if (ready()) {
                    removeListener(listener);
                    task[task.length - 1](taskCallback);
                }
            };
            addListener(listener);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.concat"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>concat ()](#apidoc.element.nodeunit.async.concat)
- description and source-code
```javascript
concat = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEach].concat(args));
}
```
- example usage
```shell
...
    iterate();
};


var doParallel = function (fn) {
    return function () {
        var args = Array.prototype.slice.call(arguments);
        return fn.apply(null, [async.forEach].concat(args));
    };
};
var doSeries = function (fn) {
    return function () {
        var args = Array.prototype.slice.call(arguments);
        return fn.apply(null, [async.forEachSeries].concat(args));
    };
...
```

#### <a name="apidoc.element.nodeunit.async.concatSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>concatSeries ()](#apidoc.element.nodeunit.async.concatSeries)
- description and source-code
```javascript
concatSeries = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEachSeries].concat(args));
}
```
- example usage
```shell
...
 * @api public
 */

exports.runSuite = function (name, suite, opt, callback) {
    suite = wrapGroup(suite);
    var keys = _keys(suite);

    async.concatSeries(keys, function (k, cb) {
var prop = suite[k], _name;

_name = name ? [].concat(name, k) : [k];
_name.toString = function () {
    // fallback for old one
    return this.join(' - ');
};
...
```

#### <a name="apidoc.element.nodeunit.async.detect"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>detect ()](#apidoc.element.nodeunit.async.detect)
- description and source-code
```javascript
detect = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEach].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.detectSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>detectSeries ()](#apidoc.element.nodeunit.async.detectSeries)
- description and source-code
```javascript
detectSeries = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEachSeries].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.dir"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>dir (fn)](#apidoc.element.nodeunit.async.dir)
- description and source-code
```javascript
dir = function (fn) {
    var args = Array.prototype.slice.call(arguments, 1);
    fn.apply(null, args.concat([function (err) {
        var args = Array.prototype.slice.call(arguments, 1);
        if (typeof console !== 'undefined') {
            if (err) {
                if (console.error) {
                    console.error(err);
                }
            }
            else if (console[name]) {
                _forEach(args, function (x) {
                    console[name](x);
                });
            }
        }
    }]));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.every"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>every (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.every)
- description and source-code
```javascript
every = function (arr, iterator, main_callback) {
    async.forEach(arr, function (x, callback) {
        iterator(x, function (v) {
            if (!v) {
                main_callback(false);
                main_callback = function () {};
            }
            callback();
        });
    }, function (err) {
        main_callback(true);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.filter"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>filter ()](#apidoc.element.nodeunit.async.filter)
- description and source-code
```javascript
filter = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEach].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.filterSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>filterSeries ()](#apidoc.element.nodeunit.async.filterSeries)
- description and source-code
```javascript
filterSeries = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEachSeries].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.foldl"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>foldl (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.foldl)
- description and source-code
```javascript
foldl = function (arr, memo, iterator, callback) {
    async.forEachSeries(arr, function (x, callback) {
        iterator(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.foldr"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>foldr (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.foldr)
- description and source-code
```javascript
foldr = function (arr, memo, iterator, callback) {
    var reversed = _map(arr, function (x) {
        return x;
    }).reverse();
    async.reduce(reversed, memo, iterator, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.forEach"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>forEach (arr, iterator, callback)](#apidoc.element.nodeunit.async.forEach)
- description and source-code
```javascript
forEach = function (arr, iterator, callback) {
    if (!arr.length) {
        return callback();
    }
    var completed = 0;
    _forEach(arr, function (x) {
        iterator(x, function (err) {
            if (err) {
                callback(err);
                callback = function () {};
            }
            else {
                completed += 1;
                if (completed === arr.length) {
                    callback();
                }
            }
        });
    });
}
```
- example usage
```shell
...
    return async;
};

//// cross-browser compatiblity functions ////

var _forEach = function (arr, iterator) {
    if (arr.forEach) {
        return arr.forEach(iterator);
    }
    for (var i = 0; i < arr.length; i += 1) {
        iterator(arr[i], i, arr);
    }
};

var _map = function (arr, iterator) {
...
```

#### <a name="apidoc.element.nodeunit.async.forEachSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>forEachSeries (arr, iterator, callback)](#apidoc.element.nodeunit.async.forEachSeries)
- description and source-code
```javascript
forEachSeries = function (arr, iterator, callback) {
    if (!arr.length) {
        return callback();
    }
    var completed = 0;
    var iterate = function () {
        iterator(arr[completed], function (err) {
            if (err) {
                callback(err);
                callback = function () {};
            }
            else {
                completed += 1;
                if (completed === arr.length) {
                    callback();
                }
                else {
                    iterate();
                }
            }
        });
    };
    iterate();
}
```
- example usage
```shell
...
async.map = doParallel(_asyncMap);
async.mapSeries = doSeries(_asyncMap);


// reduce only has a series version, as doing reduce in parallel won't
// work in many situations.
async.reduce = function (arr, memo, iterator, callback) {
    async.forEachSeries(arr, function (x, callback) {
        iterator(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
...
```

#### <a name="apidoc.element.nodeunit.async.inject"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>inject (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.inject)
- description and source-code
```javascript
inject = function (arr, memo, iterator, callback) {
    async.forEachSeries(arr, function (x, callback) {
        iterator(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.iterator"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>iterator (tasks)](#apidoc.element.nodeunit.async.iterator)
- description and source-code
```javascript
iterator = function (tasks) {
    var makeCallback = function (index) {
        var fn = function () {
            if (tasks.length) {
                tasks[index].apply(null, arguments);
            }
            return fn.next();
        };
        fn.next = function () {
            return (index < tasks.length - 1) ? makeCallback(index + 1): null;
        };
        return fn;
    };
    return makeCallback(0);
}
```
- example usage
```shell
...
                }
                async.nextTick(function () {
                    iterator.apply(null, args);
                });
            }
        };
    };
    wrapIterator(async.iterator(tasks))();
};

async.parallel = function (tasks, callback) {
    callback = callback || function () {};
    if (tasks.constructor === Array) {
        async.map(tasks, function (fn, callback) {
            if (fn) {
...
```

#### <a name="apidoc.element.nodeunit.async.log"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>log (fn)](#apidoc.element.nodeunit.async.log)
- description and source-code
```javascript
log = function (fn) {
    var args = Array.prototype.slice.call(arguments, 1);
    fn.apply(null, args.concat([function (err) {
        var args = Array.prototype.slice.call(arguments, 1);
        if (typeof console !== 'undefined') {
            if (err) {
                if (console.error) {
                    console.error(err);
                }
            }
            else if (console[name]) {
                _forEach(args, function (x) {
                    console[name](x);
                });
            }
        }
    }]));
}
```
- example usage
```shell
...
if it's missing:

#!/usr/bin/env node
try {
    var reporter = require('nodeunit').reporters.default;
}
catch(e) {
    console.log("Cannot find nodeunit module.");
    console.log("You can download submodules for this project by doing:");
    console.log("");
    console.log("    git submodule init");
    console.log("    git submodule update");
    console.log("");
    process.exit();
}
...
```

#### <a name="apidoc.element.nodeunit.async.map"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>map ()](#apidoc.element.nodeunit.async.map)
- description and source-code
```javascript
map = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEach].concat(args));
}
```
- example usage
```shell
...
    for (var i = 0; i < arr.length; i += 1) {
        iterator(arr[i], i, arr);
    }
};

var _map = function (arr, iterator) {
    if (arr.map) {
        return arr.map(iterator);
    }
    var results = [];
    _forEach(arr, function (x, i, a) {
        results.push(iterator(x, i, a));
    });
    return results;
};
...
```

#### <a name="apidoc.element.nodeunit.async.mapSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>mapSeries ()](#apidoc.element.nodeunit.async.mapSeries)
- description and source-code
```javascript
mapSeries = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEachSeries].concat(args));
}
```
- example usage
```shell
...
        });
    }
};

async.series = function (tasks, callback) {
    callback = callback || function () {};
    if (tasks.constructor === Array) {
        async.mapSeries(tasks, function (fn, callback) {
            if (fn) {
                fn(function (err) {
                    var args = Array.prototype.slice.call(arguments, 1);
                    if (args.length <= 1) {
                        args = args[0];
                    }
                    callback.call(null, err, args || null);
...
```

#### <a name="apidoc.element.nodeunit.async.memoize"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>memoize (fn, hasher)](#apidoc.element.nodeunit.async.memoize)
- description and source-code
```javascript
memoize = function (fn, hasher) {
    var memo = {};
    hasher = hasher || function (x) {
        return x;
    };
    return function () {
        var args = Array.prototype.slice.call(arguments);
        var callback = args.pop();
        var key = hasher.apply(null, args);
        if (key in memo) {
            callback.apply(null, memo[key]);
        }
        else {
            fn.apply(null, args.concat([function () {
                memo[key] = arguments;
                callback.apply(null, arguments);
            }]));
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.nextTick"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>nextTick (fn)](#apidoc.element.nodeunit.async.nextTick)
- description and source-code
```javascript
nextTick = function (fn) {
    setImmediate(fn);
}
```
- example usage
```shell
...
                var next = iterator.next();
                if (next) {
                    args.push(wrapIterator(next));
                }
                else {
                    args.push(callback);
                }
                async.nextTick(function () {
                    iterator.apply(null, args);
                });
            }
        };
    };
    wrapIterator(async.iterator(tasks))();
};
...
```

#### <a name="apidoc.element.nodeunit.async.noConflict"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>noConflict ()](#apidoc.element.nodeunit.async.noConflict)
- description and source-code
```javascript
noConflict = function () {
    root.async = previous_async;
    return async;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.parallel"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>parallel (tasks, callback)](#apidoc.element.nodeunit.async.parallel)
- description and source-code
```javascript
parallel = function (tasks, callback) {
    callback = callback || function () {};
    if (tasks.constructor === Array) {
        async.map(tasks, function (fn, callback) {
            if (fn) {
                fn(function (err) {
                    var args = Array.prototype.slice.call(arguments, 1);
                    if (args.length <= 1) {
                        args = args[0];
                    }
                    callback.call(null, err, args || null);
                });
            }
        }, callback);
    }
    else {
        var results = {};
        async.forEach(_keys(tasks), function (k, callback) {
            tasks[k](function (err) {
                var args = Array.prototype.slice.call(arguments, 1);
                if (args.length <= 1) {
                    args = args[0];
                }
                results[k] = args;
                callback(err);
            });
        }, function (err) {
            callback(err, results);
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.queue"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>queue (worker, concurrency)](#apidoc.element.nodeunit.async.queue)
- description and source-code
```javascript
queue = function (worker, concurrency) {
    var workers = 0;
    var tasks = [];
    var q = {
        concurrency: concurrency,
        push: function (data, callback) {
            tasks.push({data: data, callback: callback});
            async.nextTick(q.process);
        },
        process: function () {
            if (workers < q.concurrency && tasks.length) {
                var task = tasks.splice(0, 1)[0];
                workers += 1;
                worker(task.data, function () {
                    workers -= 1;
                    if (task.callback) {
                        task.callback.apply(task, arguments);
                    }
                    q.process();
                });
            }
        },
        length: function () {
            return tasks.length;
        }
    };
    return q;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.reduce"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>reduce (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.reduce)
- description and source-code
```javascript
reduce = function (arr, memo, iterator, callback) {
    async.forEachSeries(arr, function (x, callback) {
        iterator(memo, x, function (err, v) {
            memo = v;
            callback(err);
        });
    }, function (err) {
        callback(err, memo);
    });
}
```
- example usage
```shell
...
        results.push(iterator(x, i, a));
    });
    return results;
};

var _reduce = function (arr, iterator, memo) {
    if (arr.reduce) {
        return arr.reduce(iterator, memo);
    }
    _forEach(arr, function (x, i, a) {
        memo = iterator(memo, x, i, a);
    });
    return memo;
};
...
```

#### <a name="apidoc.element.nodeunit.async.reduceRight"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>reduceRight (arr, memo, iterator, callback)](#apidoc.element.nodeunit.async.reduceRight)
- description and source-code
```javascript
reduceRight = function (arr, memo, iterator, callback) {
    var reversed = _map(arr, function (x) {
        return x;
    }).reverse();
    async.reduce(reversed, memo, iterator, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.reject"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>reject ()](#apidoc.element.nodeunit.async.reject)
- description and source-code
```javascript
reject = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEach].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.rejectSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>rejectSeries ()](#apidoc.element.nodeunit.async.rejectSeries)
- description and source-code
```javascript
rejectSeries = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEachSeries].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.select"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>select ()](#apidoc.element.nodeunit.async.select)
- description and source-code
```javascript
select = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEach].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.selectSeries"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>selectSeries ()](#apidoc.element.nodeunit.async.selectSeries)
- description and source-code
```javascript
selectSeries = function () {
    var args = Array.prototype.slice.call(arguments);
    return fn.apply(null, [async.forEachSeries].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.series"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>series (tasks, callback)](#apidoc.element.nodeunit.async.series)
- description and source-code
```javascript
series = function (tasks, callback) {
    callback = callback || function () {};
    if (tasks.constructor === Array) {
        async.mapSeries(tasks, function (fn, callback) {
            if (fn) {
                fn(function (err) {
                    var args = Array.prototype.slice.call(arguments, 1);
                    if (args.length <= 1) {
                        args = args[0];
                    }
                    callback.call(null, err, args || null);
                });
            }
        }, callback);
    }
    else {
        var results = {};
        async.forEachSeries(_keys(tasks), function (k, callback) {
            tasks[k](function (err) {
                var args = Array.prototype.slice.call(arguments, 1);
                if (args.length <= 1) {
                    args = args[0];
                }
                results[k] = args;
                callback(err);
            });
        }, function (err) {
            callback(err, results);
        });
    }
}
```
- example usage
```shell
...
       for (var i = 0, len = fns.length; i < len; i++) {
           (function (j) {
               bound_fns.push(function () {
                   return fns[j].apply(that, arguments);
               });
           })(i);
       }
       return async.series(bound_fns, callback);
   };
};


/**
* Wraps a group of tests with setUp and tearDown functions.
* Used by testCase.
...
```

#### <a name="apidoc.element.nodeunit.async.some"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>some (arr, iterator, main_callback)](#apidoc.element.nodeunit.async.some)
- description and source-code
```javascript
some = function (arr, iterator, main_callback) {
    async.forEach(arr, function (x, callback) {
        iterator(x, function (v) {
            if (v) {
                main_callback(true);
                main_callback = function () {};
            }
            callback();
        });
    }, function (err) {
        main_callback(false);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.sortBy"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>sortBy (arr, iterator, callback)](#apidoc.element.nodeunit.async.sortBy)
- description and source-code
```javascript
sortBy = function (arr, iterator, callback) {
    async.map(arr, function (x, callback) {
        iterator(x, function (err, criteria) {
            if (err) {
                callback(err);
            }
            else {
                callback(null, {value: x, criteria: criteria});
            }
        });
    }, function (err, results) {
        if (err) {
            return callback(err);
        }
        else {
            var fn = function (left, right) {
                var a = left.criteria, b = right.criteria;
                return a < b ? -1 : a > b ? 1 : 0;
            };
            callback(null, _map(results.sort(fn), function (x) {
                return x.value;
            }));
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.until"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>until (test, iterator, callback)](#apidoc.element.nodeunit.async.until)
- description and source-code
```javascript
until = function (test, iterator, callback) {
    if (!test()) {
        iterator(function (err) {
            if (err) {
                return callback(err);
            }
            async.until(test, iterator, callback);
        });
    }
    else {
        callback();
    }
}
```
- example usage
```shell
...

async.until = function (test, iterator, callback) {
    if (!test()) {
        iterator(function (err) {
            if (err) {
                return callback(err);
            }
            async.until(test, iterator, callback);
        });
    }
    else {
        callback();
    }
};
...
```

#### <a name="apidoc.element.nodeunit.async.waterfall"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>waterfall (tasks, callback)](#apidoc.element.nodeunit.async.waterfall)
- description and source-code
```javascript
waterfall = function (tasks, callback) {
    if (!tasks.length) {
        return callback();
    }
    callback = callback || function () {};
    var wrapIterator = function (iterator) {
        return function (err) {
            if (err) {
                callback(err);
                callback = function () {};
            }
            else {
                var args = Array.prototype.slice.call(arguments, 1);
                var next = iterator.next();
                if (next) {
                    args.push(wrapIterator(next));
                }
                else {
                    args.push(callback);
                }
                async.nextTick(function () {
                    iterator.apply(null, args);
                });
            }
        };
    };
    wrapIterator(async.iterator(tasks))();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.async.whilst"></a>[function <span class="apidocSignatureSpan">nodeunit.async.</span>whilst (test, iterator, callback)](#apidoc.element.nodeunit.async.whilst)
- description and source-code
```javascript
whilst = function (test, iterator, callback) {
    if (test()) {
        iterator(function (err) {
            if (err) {
                return callback(err);
            }
            async.whilst(test, iterator, callback);
        });
    }
    else {
        callback();
    }
}
```
- example usage
```shell
...

async.whilst = function (test, iterator, callback) {
    if (test()) {
        iterator(function (err) {
            if (err) {
                return callback(err);
            }
            async.whilst(test, iterator, callback);
        });
    }
    else {
        callback();
    }
};
...
```



# <a name="apidoc.module.nodeunit.core"></a>[module nodeunit.core](#apidoc.module.nodeunit.core)

#### <a name="apidoc.element.nodeunit.core.runModule"></a>[function <span class="apidocSignatureSpan">nodeunit.core.</span>runModule (name, mod, opt, callback)](#apidoc.element.nodeunit.core.runModule)
- description and source-code
```javascript
runModule = function (name, mod, opt, callback) {
    var options = _copy(types.options(opt));

    var _run = false;
    var _moduleStart = options.moduleStart;

    mod = wrapGroup(mod);

    function run_once() {
        if (!_run) {
            _run = true;
            _moduleStart(name);
        }
    }
    options.moduleStart = run_once;

    var start = new Date().getTime();

    exports.runSuite(null, mod, options, function (err, a_list) {
        var end = new Date().getTime();
        var assertion_list = types.assertionList(a_list, end - start);
        options.moduleDone(name, assertion_list);
        if (nodeunit.complete) {
            nodeunit.complete(name, assertion_list);
        }
        callback(null, a_list);
    });
}
```
- example usage
```shell
...
// TODO: add proper unit tests for this function
exports.runModules = function (modules, opt) {
    var all_assertions = [];
    var options = types.options(opt);
    var start = new Date().getTime();

    async.concatSeries(_keys(modules), function (k, cb) {
        exports.runModule(k, modules[k], options, cb);
    },
    function (err, all_assertions) {
        var end = new Date().getTime();
        options.done(types.assertionList(all_assertions, end - start));
    });
};
...
```

#### <a name="apidoc.element.nodeunit.core.runModules"></a>[function <span class="apidocSignatureSpan">nodeunit.core.</span>runModules (modules, opt)](#apidoc.element.nodeunit.core.runModules)
- description and source-code
```javascript
runModules = function (modules, opt) {
    var all_assertions = [];
    var options = types.options(opt);
    var start = new Date().getTime();

    async.concatSeries(_keys(modules), function (k, cb) {
        exports.runModule(k, modules[k], options, cb);
    },
    function (err, all_assertions) {
        var end = new Date().getTime();
        options.done(types.assertionList(all_assertions, end - start));
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.core.runSuite"></a>[function <span class="apidocSignatureSpan">nodeunit.core.</span>runSuite (name, suite, opt, callback)](#apidoc.element.nodeunit.core.runSuite)
- description and source-code
```javascript
runSuite = function (name, suite, opt, callback) {
    suite = wrapGroup(suite);
    var keys = _keys(suite);

    async.concatSeries(keys, function (k, cb) {
        var prop = suite[k], _name;

        _name = name ? [].concat(name, k) : [k];
        _name.toString = function () {
            // fallback for old one
            return this.join(' - ');
        };

        if (typeof prop === 'function') {
            var in_name = false,
                in_specific_test = (_name.toString() === opt.testFullSpec) ? true : false;
            for (var i = 0; i < _name.length; i += 1) {
                if (_name[i] === opt.testspec) {
                    in_name = true;
                }
            }

            if ((!opt.testFullSpec || in_specific_test) && (!opt.testspec || in_name)) {
                if (opt.moduleStart) {
                    opt.moduleStart();
                }
                exports.runTest(_name, suite[k], opt, cb);
            }
            else {
                return cb();
            }
        }
        else {
            exports.runSuite(_name, suite[k], opt, cb);
        }
    }, callback);
}
```
- example usage
```shell
...
               exports.runTest(_name, suite[k], opt, cb);
           }
           else {
               return cb();
           }
       }
       else {
           exports.runSuite(_name, suite[k], opt, cb);
       }
   }, callback);
};

/**
* Run each exported test function or test suite from a loaded module.
*
...
```

#### <a name="apidoc.element.nodeunit.core.runTest"></a>[function <span class="apidocSignatureSpan">nodeunit.core.</span>runTest (name, fn, opt, callback)](#apidoc.element.nodeunit.core.runTest)
- description and source-code
```javascript
runTest = function (name, fn, opt, callback) {
    var options = types.options(opt);

    options.testStart(name);
    var start = new Date().getTime();
    var test = types.test(name, start, options, callback);

    options.testReady(test);
    try {
        fn(test);
    }
    catch (e) {
        test.done(e);
    }
}
```
- example usage
```shell
...
        }
    }

    if ((!opt.testFullSpec || in_specific_test) && (!opt.testspec || in_name)) {
        if (opt.moduleStart) {
            opt.moduleStart();
        }
        exports.runTest(_name, suite[k], opt, cb);
    }
    else {
        return cb();
    }
}
else {
    exports.runSuite(_name, suite[k], opt, cb);
...
```

#### <a name="apidoc.element.nodeunit.core.testCase"></a>[function <span class="apidocSignatureSpan">nodeunit.core.</span>testCase (suite)](#apidoc.element.nodeunit.core.testCase)
- description and source-code
```javascript
testCase = function (suite) {
    return suite;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodeunit.testrunner"></a>[module nodeunit.testrunner](#apidoc.module.nodeunit.testrunner)

#### <a name="apidoc.element.nodeunit.testrunner.run"></a>[function <span class="apidocSignatureSpan">nodeunit.testrunner.</span>run ()](#apidoc.element.nodeunit.testrunner.run)
- description and source-code
```javascript
run = function () {
    console.log(
        'WARNING: nodeunit.testrunner is going to be deprecated, please ' +
        'use nodeunit.reporters.default instead!'
    );
    return reporters['default'].run.apply(this, arguments);
}
```
- example usage
```shell
...
    <script src="nodeunit.js"></script>
    <script src="suite1.js"></script>
    <script src="suite2.js"></script>
  </head>
  <body>
    <h1 id="nodeunit-header">Example Test Suite</h1>
    <script>
      nodeunit.run({
        'Suite One': suite1,
        'Suite Two': suite2
      });
    </script>
  </body>
</html>
...
```



# <a name="apidoc.module.nodeunit.track"></a>[module nodeunit.track](#apidoc.module.nodeunit.track)

#### <a name="apidoc.element.nodeunit.track.createTracker"></a>[function <span class="apidocSignatureSpan">nodeunit.track.</span>createTracker (on_exit)](#apidoc.element.nodeunit.track.createTracker)
- description and source-code
```javascript
createTracker = function (on_exit) {
    var names = {};
    var tracker = {
        names: function () {
            var arr = [];
            for (var k in names) {
                if (names.hasOwnProperty(k)) {
                    arr.push(k);
                }
            }
            return arr;
        },
        unfinished: function () {
            return tracker.names().length;
        },
        put: function (testname) {
            names[testname] = testname;
        },
        remove: function (testname) {
            delete names[testname];
        }
    };

    process.on('exit', function() {
        on_exit = on_exit || exports.default_on_exit;
        on_exit(tracker);
    });

    return tracker;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.track.default_on_exit"></a>[function <span class="apidocSignatureSpan">nodeunit.track.</span>default_on_exit (tracker)](#apidoc.element.nodeunit.track.default_on_exit)
- description and source-code
```javascript
default_on_exit = function (tracker) {
    if (tracker.unfinished()) {
        console.log('');
        console.log('Undone tests (or their setups/teardowns): ');
        var names = tracker.names();
        for (var i = 0; i < names.length; i += 1) {
            console.log(names[i]);
        }
        process.reallyExit(tracker.unfinished());
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nodeunit.types"></a>[module nodeunit.types](#apidoc.module.nodeunit.types)

#### <a name="apidoc.element.nodeunit.types.assertion"></a>[function <span class="apidocSignatureSpan">nodeunit.types.</span>assertion (obj)](#apidoc.element.nodeunit.types.assertion)
- description and source-code
```javascript
assertion = function (obj) {
    return {
        method: obj.method || '',
        message: obj.message || (obj.error && obj.error.message) || '',
        error: obj.error,
        passed: function () {
            return !this.error;
        },
        failed: function () {
            return Boolean(this.error);
        }
    };
}
```
- example usage
```shell
...
        if (tearDown) {
var done = test.done;
test.done = function (err) {
    try {
        tearDown.call(context, function (err2) {
            if (err && err2) {
                test._assertion_list.push(
                    types.assertion({error: err})
                );
                return done(err2);
            }
            done(err || err2);
        });
    }
    catch (e) {
...
```

#### <a name="apidoc.element.nodeunit.types.assertionList"></a>[function <span class="apidocSignatureSpan">nodeunit.types.</span>assertionList (arr, duration)](#apidoc.element.nodeunit.types.assertionList)
- description and source-code
```javascript
assertionList = function (arr, duration) {
    var that = arr || [];
    that.failures = function () {
        var failures = 0;
        for (var i = 0; i < this.length; i += 1) {
            if (this[i].failed()) {
                failures += 1;
            }
        }
        return failures;
    };
    that.passes = function () {
        return that.length - that.failures();
    };
    that.duration = duration || 0;
    return that;
}
```
- example usage
```shell
...
    }
    options.moduleStart = run_once;

    var start = new Date().getTime();

    exports.runSuite(null, mod, options, function (err, a_list) {
        var end = new Date().getTime();
        var assertion_list = types.assertionList(a_list, end - start);
        options.moduleDone(name, assertion_list);
        if (nodeunit.complete) {
            nodeunit.complete(name, assertion_list);
        }
        callback(null, a_list);
    });
};
...
```

#### <a name="apidoc.element.nodeunit.types.options"></a>[function <span class="apidocSignatureSpan">nodeunit.types.</span>options (opt)](#apidoc.element.nodeunit.types.options)
- description and source-code
```javascript
options = function (opt) {
    var optionalCallback = function (name) {
        opt[name] = opt[name] || function () {};
    };

    optionalCallback('moduleStart');
    optionalCallback('moduleDone');
    optionalCallback('testStart');
    optionalCallback('testReady');
    optionalCallback('testDone');
    //optionalCallback('log');

    // 'done' callback is not optional.

    return opt;
}
```
- example usage
```shell
...
 * @param {Function} fn
 * @param {Object} opt
 * @param {Function} callback
 * @api public
 */

exports.runTest = function (name, fn, opt, callback) {
var options = types.options(opt);

options.testStart(name);
var start = new Date().getTime();
var test = types.test(name, start, options, callback);

options.testReady(test);
try {
...
```

#### <a name="apidoc.element.nodeunit.types.test"></a>[function <span class="apidocSignatureSpan">nodeunit.types.</span>test (name, start, options, callback)](#apidoc.element.nodeunit.types.test)
- description and source-code
```javascript
test = function (name, start, options, callback) {
    var expecting;
    var a_list = [];

    var wrapAssert = assertWrapper(function (a) {
        a_list.push(a);
        if (options.log) {
            async.nextTick(function () {
                options.log(a);
            });
        }
    });

    var test = {
        done: function (err) {
            if (expecting !== undefined && expecting !== a_list.length) {
                var e = new Error(
                    'Expected ' + expecting + ' assertions, ' +
                    a_list.length + ' ran'
                );
                var a1 = exports.assertion({method: 'expect', error: e});
                a_list.push(a1);
                if (options.log) {
                    async.nextTick(function () {
                        options.log(a1);
                    });
                }
            }
            if (err) {
                var a2 = exports.assertion({error: err});
                a_list.push(a2);
                if (options.log) {
                    async.nextTick(function () {
                        options.log(a2);
                    });
                }
            }
            var end = new Date().getTime();
            async.nextTick(function () {
                var assertion_list = exports.assertionList(a_list, end - start);
                options.testDone(name, assertion_list);
                callback(null, a_list);
            });
        },
        ok: wrapAssert('ok', 'ok', 2),
        same: wrapAssert('same', 'deepEqual', 3),
        equals: wrapAssert('equals', 'equal', 3),
        expect: function (num) {
            expecting = num;
        },
        _assertion_list: a_list
    };
    // add all functions from the assert module
    for (var k in assert) {
        if (assert.hasOwnProperty(k)) {
            test[k] = wrapAssert(k, k, assert[k].length);
        }
    }
    return test;
}
```
- example usage
```shell
...

// If the string contains no control characters, no quote characters, and no
// backslash characters, then we can safely slap some quotes around it.
// Otherwise we must also replace the offending characters with safe escape
// sequences.

    escapable.lastIndex = 0;
    return escapable.test(string) ?
        '"' + string.replace(escapable, function (a) {
            var c = meta[a];
            return typeof c === 'string' ? c :
                '\\u' + ('0000' + a.charCodeAt(0).toString(16)).slice(-4);
        }) + '"' :
        '"' + string + '"';
}
...
```



# <a name="apidoc.module.nodeunit.utils"></a>[module nodeunit.utils](#apidoc.module.nodeunit.utils)

#### <a name="apidoc.element.nodeunit.utils.betterErrors"></a>[function <span class="apidocSignatureSpan">nodeunit.utils.</span>betterErrors (assertion)](#apidoc.element.nodeunit.utils.betterErrors)
- description and source-code
```javascript
betterErrors = function (assertion) {
    if (!assertion.error) {
        return assertion;
    }
    var e = assertion.error;

    if (typeof e.actual !== 'undefined' && typeof e.expected !== 'undefined') {
        var actual = util.inspect(e.actual, false, 10).replace(/\n$/, '');
        var expected = util.inspect(e.expected, false, 10).replace(/\n$/, '');

        var multiline = (
            actual.indexOf('\n') !== -1 ||
            expected.indexOf('\n') !== -1
        );
        var spacing = (multiline ? '\n' : ' ');
        e._message = e.message;
        e.stack = (
            e.name + ':' + spacing +
            actual + spacing + e.operator + spacing +
            expected + '\n' +
            e.stack.split('\n').slice(1).join('\n')
        );
    }
    return assertion;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.utils.httputil"></a>[function <span class="apidocSignatureSpan">nodeunit.utils.</span>httputil (cgi, envReady)](#apidoc.element.nodeunit.utils.httputil)
- description and source-code
```javascript
httputil = function (cgi, envReady) {
    var hostname = process.env.HOSTNAME || 'localhost';
    var port = process.env.PORT || 3000;

    var server = http.createServer(cgi);
    server.listen(port, hostname);

    var agent = new http.Agent({ host: hostname, port: port, maxSockets: 1 });
    var client = {
        fetch: function (method, path, headers, respReady) {
            var request = http.request({
                host: hostname,
                port: port,
                agent: agent,
                method: method,
                path: path,
                headers: headers
            });
            request.end();
            request.on('response', function (response) {
                response.setEncoding('utf8');
                response.on('data', function (chunk) {
                    if (response.body) {
                        response.body += chunk;
                    } else {
                        response.body = chunk;
                    }
                });
                response.on('end', function () {
                    if (response.headers['content-type'] === 'application/json') {
                        response.bodyAsObject = JSON.parse(response.body);
                    }
                    respReady(response);
                });
            });
        }
    };

    process.nextTick(function () {
        if (envReady && typeof envReady === 'function') {
            envReady(server, client);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.utils.modulePaths"></a>[function <span class="apidocSignatureSpan">nodeunit.utils.</span>modulePaths (paths, callback, recursive)](#apidoc.element.nodeunit.utils.modulePaths)
- description and source-code
```javascript
function modulePaths(paths, callback, recursive) {
    recursive = (recursive === true);
    async.concatSeries(paths, function (p, cb) {
        fs.stat(p, function (err, stats) {
            if (err) {
                return cb(err);
            }
            if (stats.isFile()) {
                return cb(null, [p]);
            }
            if (stats.isDirectory()) {
                fs.readdir(p, function (err, files) {
                    if (err) {
                        return cb(err);
                    }

                    // filter out any filenames with unsupported extensions
                    var modules = files.filter(function (filename) {
                        return extensionPattern.exec(filename);
                    });

                    // remove extension from module name and prepend the
                    // directory path
                    var fullpaths = modules.map(function (filename) {
                        var mod_name = filename.replace(extensionPattern, '');
                        return [p, mod_name].join('/');
                    });

                    if (recursive) {
                        // get all sub directories
                        var directories =
                            files
                                .map(function(filename) {
                                    // resolve path first
                                    return path.resolve(p, filename);
                                })
                                .filter(function(filename) {
                                    // fetch only directories
                                    return (fs.statSync(filename).isDirectory());
                                });

                        // recursively call modulePaths() with sub directories
                        modulePaths(directories, function(err, files) {
                            if (!err) {
                                cb(null, fullpaths.concat(files).sort())
                            } else {
                                cb(err);
                            }
                        }, recursive);
                    } else {
                        // sort filenames here, because Array.map changes order
                        fullpaths.sort();

                        // finish
                        cb(null, fullpaths);
                    }

                });
            }
        });
    }, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nodeunit.utils.sandbox"></a>[function <span class="apidocSignatureSpan">nodeunit.utils.</span>sandbox (files, sandbox)](#apidoc.element.nodeunit.utils.sandbox)
- description and source-code
```javascript
sandbox = function (files, sandbox) {
    var source, script, result;
    if (!(files instanceof Array)) {
        files = [files];
    }
    source = files.map(function (file) {
        return fs.readFileSync(file, 'utf8');
    }).join('');

    if (!sandbox) {
        sandbox = {};
    }
    script = new Script(source);
    result = script.runInNewContext(sandbox);
    return sandbox;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
