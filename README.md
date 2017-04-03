# api documentation for  [monk (v4.0.0)](https://github.com/Automattic/monk#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-monk.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-monk) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-monk.svg)](https://travis-ci.org/npmdoc/node-npmdoc-monk)
#### [![build status](https://secure.travis-ci.org/Automattic/monk.svg?branch=master)](https://secure.travis-ci.org/Automattic/monk) [![codecov](https://codecov.io/gh/Automattic/monk/branch/master/graph/badge.svg)](https://codecov.io/gh/Automattic/monk) [![Joi

[![NPM](https://nodei.co/npm/monk.png?downloads=true)](https://www.npmjs.com/package/monk)

[![apidoc](https://npmdoc.github.io/node-npmdoc-monk/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-monk_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-monk/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-monk/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-monk/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/Automattic/monk/issues"
    },
    "dependencies": {
        "debug": "*",
        "mongodb": "^2.1.18"
    },
    "description": "[![build status](https://secure.travis-ci.org/Automattic/monk.svg?branch=master)](https://secure.travis-ci.org/Automattic/monk) [![codecov](https://codecov.io/gh/Automattic/monk/branch/master/graph/badge.svg)](https://codecov.io/gh/Automattic/monk) [![Joi",
    "devDependencies": {
        "ava": "^0.15.2",
        "codecov": "^1.0.1",
        "eslint": "^2.11.1",
        "eslint-config-standard": "^5.3.1",
        "eslint-plugin-ava": "2.5.0",
        "eslint-plugin-promise": "^1.3.2",
        "eslint-plugin-standard": "^1.3.2",
        "gitbook-cli": "2.3.0",
        "gitbook-plugin-anker-enable": "0.0.4",
        "gitbook-plugin-edit-link": "2.0.2",
        "gitbook-plugin-github": "2.0.0",
        "gitbook-plugin-prism": "1.0.0",
        "nyc": "^6.4.4"
    },
    "directories": {},
    "dist": {
        "shasum": "ac5439e3543b1b486d787d1704bd7e10a2ddd0d2",
        "tarball": "https://registry.npmjs.org/monk/-/monk-4.0.0.tgz"
    },
    "files": [
        "lib"
    ],
    "gitHead": "88caf69ad0da0d3d4691a4affa5181e290340c25",
    "homepage": "https://github.com/Automattic/monk#readme",
    "license": "MIT",
    "main": "lib/monk.js",
    "maintainers": [
        {
            "name": "mathieudutour",
            "email": "mathieu@dutour.me"
        },
        {
            "name": "rauchg",
            "email": "rauchg@gmail.com"
        },
        {
            "name": "tootallnate",
            "email": "nathan@tootallnate.net"
        }
    ],
    "name": "monk",
    "nyc": {
        "include": [
            "lib/**"
        ]
    },
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/Automattic/monk.git"
    },
    "scripts": {
        "coverage": "nyc report --reporter=text-lcov > coverage.lcov && codecov",
        "test": "make test"
    },
    "tags": [
        "mongodb",
        "mongo",
        "driver"
    ],
    "version": "4.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module monk](#apidoc.module.monk)
1.  [function <span class="apidocSignatureSpan">monk.</span>Collection (manager, name, options)](#apidoc.element.monk.Collection)
1.  [function <span class="apidocSignatureSpan">monk.</span>id (str)](#apidoc.element.monk.id)
1.  [function <span class="apidocSignatureSpan">monk.</span>super_ ()](#apidoc.element.monk.super_)
1.  object <span class="apidocSignatureSpan">monk.</span>Collection.prototype
1.  object <span class="apidocSignatureSpan">monk.</span>helpers
1.  object <span class="apidocSignatureSpan">monk.</span>util

#### [module monk.Collection](#apidoc.module.monk.Collection)
1.  [function <span class="apidocSignatureSpan">monk.</span>Collection (manager, name, options)](#apidoc.element.monk.Collection.Collection)

#### [module monk.Collection.prototype](#apidoc.module.monk.Collection.prototype)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>aggregate (stages, opts, fn)](#apidoc.element.monk.Collection.prototype.aggregate)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>bulkWrite (operations, opts, fn)](#apidoc.element.monk.Collection.prototype.bulkWrite)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>count (query, opts, fn)](#apidoc.element.monk.Collection.prototype.count)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>distinct (field, query, opts, fn)](#apidoc.element.monk.Collection.prototype.distinct)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>drop (fn)](#apidoc.element.monk.Collection.prototype.drop)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>dropIndex (fields, opts, fn)](#apidoc.element.monk.Collection.prototype.dropIndex)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>dropIndexes (fn)](#apidoc.element.monk.Collection.prototype.dropIndexes)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>ensureIndex (fields, opts, fn)](#apidoc.element.monk.Collection.prototype.ensureIndex)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>executeWhenOpened (fn)](#apidoc.element.monk.Collection.prototype.executeWhenOpened)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>find (query, opts, fn)](#apidoc.element.monk.Collection.prototype.find)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findAndModify (query, update, opts, fn)](#apidoc.element.monk.Collection.prototype.findAndModify)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findById (id, opts, fn)](#apidoc.element.monk.Collection.prototype.findById)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findOne (query, opts, fn)](#apidoc.element.monk.Collection.prototype.findOne)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findOneAndDelete (query, opts, fn)](#apidoc.element.monk.Collection.prototype.findOneAndDelete)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findOneAndUpdate (query, update, opts, fn)](#apidoc.element.monk.Collection.prototype.findOneAndUpdate)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>group (keys, condition, initial, reduce, finalize, command, opts, fn)](#apidoc.element.monk.Collection.prototype.group)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>id (str)](#apidoc.element.monk.Collection.prototype.id)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>indexes (fn)](#apidoc.element.monk.Collection.prototype.indexes)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>insert (data, opts, fn)](#apidoc.element.monk.Collection.prototype.insert)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>opts (opts)](#apidoc.element.monk.Collection.prototype.opts)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>remove (query, opts, fn)](#apidoc.element.monk.Collection.prototype.remove)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>removeById (id, opts, fn)](#apidoc.element.monk.Collection.prototype.removeById)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>update (query, update, opts, fn)](#apidoc.element.monk.Collection.prototype.update)
1.  [function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>updateById (id, update, opts, fn)](#apidoc.element.monk.Collection.prototype.updateById)

#### [module monk.helpers](#apidoc.module.monk.helpers)
1.  [function <span class="apidocSignatureSpan">monk.helpers.</span>id (str)](#apidoc.element.monk.helpers.id)

#### [module monk.util](#apidoc.module.monk.util)
1.  [function <span class="apidocSignatureSpan">monk.util.</span>cast (obj)](#apidoc.element.monk.util.cast)
1.  [function <span class="apidocSignatureSpan">monk.util.</span>fields (obj, numberWhenMinus)](#apidoc.element.monk.util.fields)
1.  [function <span class="apidocSignatureSpan">monk.util.</span>options (opts)](#apidoc.element.monk.util.options)
1.  [function <span class="apidocSignatureSpan">monk.util.</span>query (query)](#apidoc.element.monk.util.query)



# <a name="apidoc.module.monk"></a>[module monk](#apidoc.module.monk)

#### <a name="apidoc.element.monk.Collection"></a>[function <span class="apidocSignatureSpan">monk.</span>Collection (manager, name, options)](#apidoc.element.monk.Collection)
- description and source-code
```javascript
function Collection(manager, name, options) {
  this.manager = manager
  this.name = name
  this.options = options || {}

  delete this.options.cache

  this.oid = this.id
  this.opts = this.opts.bind(this)
  this.index = this.ensureIndex = this.ensureIndex.bind(this)
  this.dropIndex = this.dropIndex.bind(this)
  this.indexes = this.indexes.bind(this)
  this.dropIndexes = this.dropIndexes.bind(this)
  this.update = this.update.bind(this)
  this.updateById = this.updateById.bind(this)
  this.remove = this.remove.bind(this)
  this.removeById = this.removeById.bind(this)
  this.findAndModify = this.findAndModify.bind(this)
  this.findOneAndUpdate = this.findOneAndUpdate.bind(this)
  this.findOneAndDelete = this.findOneAndDelete.bind(this)
  this.insert = this.insert.bind(this)
  this.findById = this.findById.bind(this)
  this.find = this.find.bind(this)
  this.distinct = this.distinct.bind(this)
  this.count = this.count.bind(this)
  this.findOne = this.findOne.bind(this)
  this.aggregate = this.aggregate.bind(this)
  this.drop = this.drop.bind(this)
  util.cast = util.cast.bind(this)
  this.executeWhenOpened = this.executeWhenOpened.bind(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.id"></a>[function <span class="apidocSignatureSpan">monk.</span>id (str)](#apidoc.element.monk.id)
- description and source-code
```javascript
id = function (str) {
  if (str == null) return ObjectId()
  return typeof str === 'string' ? ObjectId.createFromHexString(str) : str
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.super_"></a>[function <span class="apidocSignatureSpan">monk.</span>super_ ()](#apidoc.element.monk.super_)
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



# <a name="apidoc.module.monk.Collection"></a>[module monk.Collection](#apidoc.module.monk.Collection)

#### <a name="apidoc.element.monk.Collection.Collection"></a>[function <span class="apidocSignatureSpan">monk.</span>Collection (manager, name, options)](#apidoc.element.monk.Collection.Collection)
- description and source-code
```javascript
function Collection(manager, name, options) {
  this.manager = manager
  this.name = name
  this.options = options || {}

  delete this.options.cache

  this.oid = this.id
  this.opts = this.opts.bind(this)
  this.index = this.ensureIndex = this.ensureIndex.bind(this)
  this.dropIndex = this.dropIndex.bind(this)
  this.indexes = this.indexes.bind(this)
  this.dropIndexes = this.dropIndexes.bind(this)
  this.update = this.update.bind(this)
  this.updateById = this.updateById.bind(this)
  this.remove = this.remove.bind(this)
  this.removeById = this.removeById.bind(this)
  this.findAndModify = this.findAndModify.bind(this)
  this.findOneAndUpdate = this.findOneAndUpdate.bind(this)
  this.findOneAndDelete = this.findOneAndDelete.bind(this)
  this.insert = this.insert.bind(this)
  this.findById = this.findById.bind(this)
  this.find = this.find.bind(this)
  this.distinct = this.distinct.bind(this)
  this.count = this.count.bind(this)
  this.findOne = this.findOne.bind(this)
  this.aggregate = this.aggregate.bind(this)
  this.drop = this.drop.bind(this)
  util.cast = util.cast.bind(this)
  this.executeWhenOpened = this.executeWhenOpened.bind(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monk.Collection.prototype"></a>[module monk.Collection.prototype](#apidoc.module.monk.Collection.prototype)

#### <a name="apidoc.element.monk.Collection.prototype.aggregate"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>aggregate (stages, opts, fn)](#apidoc.element.monk.Collection.prototype.aggregate)
- description and source-code
```javascript
aggregate = function (stages, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  // opts
  opts = this.opts(opts)

  // query
  debug('%s aggregate %j', this.name, stages)
  return this.executeWhenOpened().then(function (col) {
    return col.aggregate(stages, opts)
  }).then(function (cursor) {
    return cursor.toArray()
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.bulkWrite"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>bulkWrite (operations, opts, fn)](#apidoc.element.monk.Collection.prototype.bulkWrite)
- description and source-code
```javascript
bulkWrite = function (operations, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    operations = util.cast(operations)
  }

  // query
  debug('%s bulkWrite %j', this.name, operations)
  return this.executeWhenOpened().then(function (col) {
    return col.bulkWrite(operations, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.count"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>count (query, opts, fn)](#apidoc.element.monk.Collection.prototype.count)
- description and source-code
```javascript
count = function (query, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  // opts
  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s count %j', this.name, query)
  return this.executeWhenOpened().then(function (col) {
    return col.count(query, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.distinct"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>distinct (field, query, opts, fn)](#apidoc.element.monk.Collection.prototype.distinct)
- description and source-code
```javascript
distinct = function (field, query, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  if (typeof query === 'function') {
    fn = query
    query = {}
  }

  query = util.query(query)

  // opts
  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s distinct %s (%j)', this.name, field, query)
  return this.executeWhenOpened().then(function (col) {
    return col.distinct(field, query, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.drop"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>drop (fn)](#apidoc.element.monk.Collection.prototype.drop)
- description and source-code
```javascript
drop = function (fn) {
  debug('%s drop', this.name)
  return this.executeWhenOpened().then(function (col) {
    return col.drop()
  }).catch(function (err) {
    if (err && err.message === 'ns not found') {
      return 'ns not found'
    } else {
      throw err
    }
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.dropIndex"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>dropIndex (fields, opts, fn)](#apidoc.element.monk.Collection.prototype.dropIndex)
- description and source-code
```javascript
dropIndex = function (fields, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  fields = util.fields(fields)
  opts = this.opts(opts)

  // query
  debug('%s dropIndex %j (%j)', this.name, fields, opts)
  return this.executeWhenOpened().then(function (col) {
    return col.dropIndex(fields, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.dropIndexes"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>dropIndexes (fn)](#apidoc.element.monk.Collection.prototype.dropIndexes)
- description and source-code
```javascript
dropIndexes = function (fn) {
  // query
  debug('%s dropIndexes', this.name)
  return this.executeWhenOpened().then(function (col) {
    return col.dropIndexes()
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.ensureIndex"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>ensureIndex (fields, opts, fn)](#apidoc.element.monk.Collection.prototype.ensureIndex)
- description and source-code
```javascript
ensureIndex = function (fields, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  fields = util.fields(fields)

  // query
  debug('%s ensureIndex %j (%j)', this.name, fields, opts)
  return this.executeWhenOpened().then(function (col) {
    return col.ensureIndex(fields, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.executeWhenOpened"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>executeWhenOpened (fn)](#apidoc.element.monk.Collection.prototype.executeWhenOpened)
- description and source-code
```javascript
executeWhenOpened = function (fn) {
  return this.manager.executeWhenOpened().then(function (db) {
    return db.collection(this.name)
  }.bind(this))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.find"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>find (query, opts, fn)](#apidoc.element.monk.Collection.prototype.find)
- description and source-code
```javascript
find = function (query, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  // opts
  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s find %j', this.name, query)

  if (opts.rawCursor) {
    delete opts.rawCursor
    return this.executeWhenOpened().then(function (col) {
      return col.find(query, opts)
    }).then(thenFn(fn)).catch(catchFn(fn))
  }

  var promise = this.executeWhenOpened().then(function (col) {
    return col.find(query, opts)
  }).then(function (cursor) {
    if (!opts.stream && !promise.eachListener) {
      return cursor.toArray().then(thenFn(fn)).catch(catchFn(fn))
    }

    if (typeof opts.stream === 'function') {
      promise.eachListener = opts.stream
    }

    var didClose = false
    var didFinish = false
    var processing = 0

    function close () {
      didClose = true
      processing -= 1
      cursor.close()
    }

    function pause () {
      processing += 1
      cursor.pause()
    }

    return new Promise(function (resolve, reject) {
      cursor.on('data', function (doc) {
        if (!didClose) {
          promise.eachListener(doc, {
            close: close,
            pause: pause,
            resume: resume
          })
        }
      })

      function resume () {
        processing -= 1
        cursor.resume()
        if (processing === 0 && didFinish) {
          done()
        }
      }

      function done () {
        didFinish = true
        if (processing <= 0) {
          if (fn) {
            fn()
          }
          resolve()
        }
      }

      cursor.on('close', done)
      cursor.on('end', done)

      cursor.on('error', function (err) {
        if (fn) {
          fn(err)
        }
        reject(err)
      })
    })
  })

  promise.each = function (eachListener) {
    promise.eachListener = eachListener
    return promise
  }

  return promise
}
```
- example usage
```shell
...

'''js
const db = require('monk')('localhost/mydb')
const users = db.get('users')

users.index('name last')
users.insert({ name: 'Tobi', bigdata: {} })
users.find({ name: 'Loki' }, '-bigdata').then(function () {
  // exclude bigdata field
})
users.find({}, {sort: {name: 1}}).then(function () {
  // sorted by name field
})
users.remove({ name: 'Loki' })
...
```

#### <a name="apidoc.element.monk.Collection.prototype.findAndModify"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findAndModify (query, update, opts, fn)](#apidoc.element.monk.Collection.prototype.findAndModify)
- description and source-code
```javascript
findAndModify = function (query, update, opts, fn) {
  query = query || {}

  if (typeof query.query !== 'object' && typeof query.update !== 'object') {
    query = {
      query: query,
      update: update
    }
  } else {
    fn = opts
    opts = update
  }

  query.query = util.query(query.query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  if (opts.remove) {
    console.warn('DEPRECATED (collection.findAndModify): use collection.findOneAndDelete instead (see https://Automattic.github.
io/monk/docs/collection/findOneAndDelete.html)')
  } else {
    console.warn('DEPRECATED (collection.findAndModify): use collection.findOneAndUpdate instead (see https://Automattic.github.
io/monk/docs/collection/findOneAndUpdate.html)')
  }

  // 'new' defaults to 'true' for upserts
  if (opts.new == null && opts.upsert) {
    opts.new = true
  }

  // cast
  if (opts.castIds !== false) {
    query.query = util.cast(query.query)
    query.update = util.cast(query.update)
  }

  // query
  debug('%s findAndModify %j with %j', this.name, query.query, query.update)
  return this.executeWhenOpened().then(function (col) {
    return col.findAndModify(
      query.query,
      [],
      query.update,
      opts
    )
  }).then(function (doc) {
    return doc && doc.value || doc
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.findById"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findById (id, opts, fn)](#apidoc.element.monk.Collection.prototype.findById)
- description and source-code
```javascript
findById = function (id, opts, fn) {
  console.warn('DEPRECATED (collection.findById): use collection.findOne instead (see https://Automattic.github.io/monk/docs/collection
/findOne.html)')
  return this.findOne({ _id: id }, opts, fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.findOne"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findOne (query, opts, fn)](#apidoc.element.monk.Collection.prototype.findOne)
- description and source-code
```javascript
findOne = function (query, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  // opts
  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s findOne %j', this.name, query)
  return this.executeWhenOpened().then(function (col) {
    return col.find(query, opts).limit(1).toArray()
  }).then(function (docs) {
    return docs && docs[0] || null
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.findOneAndDelete"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findOneAndDelete (query, opts, fn)](#apidoc.element.monk.Collection.prototype.findOneAndDelete)
- description and source-code
```javascript
findOneAndDelete = function (query, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s findOneAndDelete %j with %j', this.name, query)
  return this.executeWhenOpened().then(function (col) {
    return col.findOneAndDelete(query, opts)
  }).then(function (doc) {
    return doc && doc.value || doc
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.findOneAndUpdate"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>findOneAndUpdate (query, update, opts, fn)](#apidoc.element.monk.Collection.prototype.findOneAndUpdate)
- description and source-code
```javascript
findOneAndUpdate = function (query, update, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  if (typeof opts.returnOriginal === 'undefined') {
    opts.returnOriginal = false
  }

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s findOneAndUpdate %j with %j', this.name, query, update)
  return this.executeWhenOpened().then(function (col) {
    return col.findOneAndUpdate(query, update, opts)
  }).then(function (doc) {
    return doc && doc.value || doc
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.group"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>group (keys, condition, initial, reduce, finalize, command, opts, fn)](#apidoc.element.monk.Collection.prototype.group)
- description and source-code
```javascript
group = function (keys, condition, initial, reduce, finalize, command, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  // query
  debug('%s group %j with %j', this.name, keys, condition)
  return this.executeWhenOpened().then(function (col) {
    return col.group(keys, condition, initial, reduce, finalize, command, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.id"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>id (str)](#apidoc.element.monk.Collection.prototype.id)
- description and source-code
```javascript
id = function (str) {
  console.warn('DEPRECATED (collection.id): use monk.id instead (see https://Automattic.github.io/monk/docs/id.html)')
  return require('./helpers').id(str)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.indexes"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>indexes (fn)](#apidoc.element.monk.Collection.prototype.indexes)
- description and source-code
```javascript
indexes = function (fn) {
  debug('%s indexInformation', this.name)
  return this.executeWhenOpened().then(function (col) {
    return col.indexInformation()
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.insert"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>insert (data, opts, fn)](#apidoc.element.monk.Collection.prototype.insert)
- description and source-code
```javascript
insert = function (data, opts, fn) {
  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  var arrayInsert = Array.isArray(data)

  if (arrayInsert && data.length === 0) {
    debug('%s inserting empty array in %j', this.name)
    return Promise.resolve([])
  }

  // cast
  if (opts.castIds !== false) {
    data = util.cast(data)
  }

  // query
  debug('%s insert %j', this.name, data)
  return this.executeWhenOpened().then(function (col) {
    return col.insert(data, opts)
  }).then(function (docs) {
    var res = (docs || {}).ops
    if (res && !arrayInsert) {
      res = docs.ops[0]
    }
    return res
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
...
*note*: monk 2.x drop the support for node < 0.12. If you are still using an earlier version, stick to monk 1.x

'''js
const db = require('monk')('localhost/mydb')
const users = db.get('users')

users.index('name last')
users.insert({ name: 'Tobi', bigdata: {} })
users.find({ name: 'Loki' }, '-bigdata').then(function () {
  // exclude bigdata field
})
users.find({}, {sort: {name: 1}}).then(function () {
  // sorted by name field
})
users.remove({ name: 'Loki' })
...
```

#### <a name="apidoc.element.monk.Collection.prototype.opts"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>opts (opts)](#apidoc.element.monk.Collection.prototype.opts)
- description and source-code
```javascript
opts = function (opts) {
  opts = util.options(opts || {})

  for (var i in this.manager.options) {
    if (!(i in opts) && !(i in this.options)) {
      opts[i] = this.manager.options[i]
    }
  }

  for (var j in this.options) {
    if (!(j in opts)) {
      opts[j] = this.options[j]
    }
  }

  return opts
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.remove"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>remove (query, opts, fn)](#apidoc.element.monk.Collection.prototype.remove)
- description and source-code
```javascript
remove = function (query, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
  }

  // query
  debug('%s remove %j with %j', this.name, query, opts)
  return this.executeWhenOpened().then(function (col) {
    return col.remove(query, opts)
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
...
users.insert({ name: 'Tobi', bigdata: {} })
users.find({ name: 'Loki' }, '-bigdata').then(function () {
  // exclude bigdata field
})
users.find({}, {sort: {name: 1}}).then(function () {
  // sorted by name field
})
users.remove({ name: 'Loki' })

db.close()
'''

## Features

- Command buffering. You can start querying right away.
...
```

#### <a name="apidoc.element.monk.Collection.prototype.removeById"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>removeById (id, opts, fn)](#apidoc.element.monk.Collection.prototype.removeById)
- description and source-code
```javascript
removeById = function (id, opts, fn) {
  console.warn('DEPRECATED (collection.removeById): use collection.remove instead (see https://Automattic.github.io/monk/docs/collection
/remove.html)')
  return this.remove({ _id: id }, opts, fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.update"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>update (query, update, opts, fn)](#apidoc.element.monk.Collection.prototype.update)
- description and source-code
```javascript
update = function (query, update, opts, fn) {
  query = util.query(query)

  if (typeof opts === 'function') {
    fn = opts
    opts = {}
  }

  opts = this.opts(opts)

  // cast
  if (opts.castIds !== false) {
    query = util.cast(query)
    update = util.cast(update)
  }

  // query
  debug('%s update %j with %j', this.name, query, update)
  return this.executeWhenOpened().then(function (col) {
    return col.update(query, update, opts)
  }).then(function (doc) {
    return doc && doc.result || doc
  }).then(thenFn(fn)).catch(catchFn(fn))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.Collection.prototype.updateById"></a>[function <span class="apidocSignatureSpan">monk.Collection.prototype.</span>updateById (id, update, opts, fn)](#apidoc.element.monk.Collection.prototype.updateById)
- description and source-code
```javascript
updateById = function (id, update, opts, fn) {
  console.warn('DEPRECATED (collection.updateById): use collection.update instead (see https://Automattic.github.io/monk/docs/collection
/update.html)')
  return this.update({ _id: id }, update, opts, fn)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monk.helpers"></a>[module monk.helpers](#apidoc.module.monk.helpers)

#### <a name="apidoc.element.monk.helpers.id"></a>[function <span class="apidocSignatureSpan">monk.helpers.</span>id (str)](#apidoc.element.monk.helpers.id)
- description and source-code
```javascript
id = function (str) {
  if (str == null) return ObjectId()
  return typeof str === 'string' ? ObjectId.createFromHexString(str) : str
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.monk.util"></a>[module monk.util](#apidoc.module.monk.util)

#### <a name="apidoc.element.monk.util.cast"></a>[function <span class="apidocSignatureSpan">monk.util.</span>cast (obj)](#apidoc.element.monk.util.cast)
- description and source-code
```javascript
function cast(obj) {
  if (Array.isArray(obj)) {
    return obj.map(cast)
  }

  if (obj && typeof obj === 'object') {
    Object.keys(obj).forEach(function (k) {
      if (k === '_id' && obj._id) {
        if (obj._id.$in) {
          obj._id.$in = obj._id.$in.map(id)
        } else if (obj._id.$nin) {
          obj._id.$nin = obj._id.$nin.map(id)
        } else if (obj._id.$ne) {
          obj._id.$ne = id(obj._id.$ne)
        } else {
          obj._id = id(obj._id)
        }
      } else {
        obj[k] = cast(obj[k])
      }
    })
  }

  return obj
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.util.fields"></a>[function <span class="apidocSignatureSpan">monk.util.</span>fields (obj, numberWhenMinus)](#apidoc.element.monk.util.fields)
- description and source-code
```javascript
fields = function (obj, numberWhenMinus) {
  if (!Array.isArray(obj) && typeof obj === 'object') {
    return obj
  }

  var fields = {}
  obj = typeof obj === 'string' ? obj.split(' ') : (obj || [])

  for (var i = 0, l = obj.length; i < l; i++) {
    if (obj[i][0] === '-') {
      fields[obj[i].substr(1)] = numberWhenMinus
    } else {
      fields[obj[i]] = 1
    }
  }

  return fields
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.util.options"></a>[function <span class="apidocSignatureSpan">monk.util.</span>options (opts)](#apidoc.element.monk.util.options)
- description and source-code
```javascript
options = function (opts) {
  if (typeof opts === 'string' || Array.isArray(opts)) {
    return { fields: exports.fields(opts) }
  }
  opts = opts || {}
  opts.fields = exports.fields(opts.fields, 0)
  opts.sort = exports.fields(opts.sort, -1)
  return opts
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.monk.util.query"></a>[function <span class="apidocSignatureSpan">monk.util.</span>query (query)](#apidoc.element.monk.util.query)
- description and source-code
```javascript
query = function (query) {
  query = query || {}

  if (typeof query === 'string' || typeof query.toHexString === 'function') {
    return {_id: query}
  }

  return query
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
