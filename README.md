# api documentation for  [scuttlebutt (v5.6.14)](https://github.com/dominictarr/scuttlebutt)  [![npm package](https://img.shields.io/npm/v/npmdoc-scuttlebutt.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-scuttlebutt) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-scuttlebutt.svg)](https://travis-ci.org/npmdoc/node-npmdoc-scuttlebutt)
#### replicate data via scuttlebutt protocol

[![NPM](https://nodei.co/npm/scuttlebutt.png?downloads=true)](https://www.npmjs.com/package/scuttlebutt)

[![apidoc](https://npmdoc.github.io/node-npmdoc-scuttlebutt/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-scuttlebutt_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-scuttlebutt/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-scuttlebutt/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-scuttlebutt/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dominic Tarr",
        "email": "dominic.tarr@gmail.com",
        "url": "http://dominictarr.com"
    },
    "bugs": {
        "url": "https://github.com/dominictarr/scuttlebutt/issues"
    },
    "dependencies": {
        "duplex": "~1.0.0",
        "iterate": "0.1.0",
        "monotonic-timestamp": "~0.0.8",
        "stream-serializer": "1.1.2"
    },
    "description": "replicate data via scuttlebutt protocol",
    "devDependencies": {
        "event-stream": "~3.0",
        "macgyver": "~1.10",
        "request": "~2.16.6",
        "tape": "~0.1.5"
    },
    "directories": {},
    "dist": {
        "shasum": "480ad08f1d51da416b6414677f3e848c924e1b0a",
        "tarball": "https://registry.npmjs.org/scuttlebutt/-/scuttlebutt-5.6.14.tgz"
    },
    "gitHead": "690377c768e52df580fd01247f6e77c8e87ec154",
    "homepage": "https://github.com/dominictarr/scuttlebutt",
    "maintainers": [
        {
            "name": "dominictarr",
            "email": "dominic.tarr@gmail.com"
        }
    ],
    "name": "scuttlebutt",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/dominictarr/scuttlebutt.git"
    },
    "scripts": {
        "test": "set -e; for test in test/*.js; do node $test; done"
    },
    "testling": {
        "files": "test/*.js",
        "browsers": {
            "ie": [
                8,
                9,
                10
            ],
            "firefox": [
                17,
                18
            ],
            "chrome": [
                23,
                24
            ],
            "safari": [
                5,
                6
            ],
            "opera": [
                12
            ]
        }
    },
    "version": "5.6.14"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module scuttlebutt](#apidoc.module.scuttlebutt)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>events (opts)](#apidoc.element.scuttlebutt.events)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>filter (update, sources)](#apidoc.element.scuttlebutt.filter)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>model (opts)](#apidoc.element.scuttlebutt.model)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>super_ ()](#apidoc.element.scuttlebutt.super_)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>timestamp ()](#apidoc.element.scuttlebutt.timestamp)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>updateIsRecent (update, sources)](#apidoc.element.scuttlebutt.updateIsRecent)
1.  object <span class="apidocSignatureSpan">scuttlebutt.</span>events.prototype
1.  object <span class="apidocSignatureSpan">scuttlebutt.</span>model.prototype
1.  object <span class="apidocSignatureSpan">scuttlebutt.</span>util

#### [module scuttlebutt.events](#apidoc.module.scuttlebutt.events)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>events (opts)](#apidoc.element.scuttlebutt.events.events)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.events.</span>super_ (opts)](#apidoc.element.scuttlebutt.events.super_)

#### [module scuttlebutt.events.prototype](#apidoc.module.scuttlebutt.events.prototype)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>applyUpdate (update)](#apidoc.element.scuttlebutt.events.prototype.applyUpdate)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>emit (event)](#apidoc.element.scuttlebutt.events.prototype.emit)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>history (filter)](#apidoc.element.scuttlebutt.events.prototype.history)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>on (event, listener)](#apidoc.element.scuttlebutt.events.prototype.on)

#### [module scuttlebutt.model](#apidoc.module.scuttlebutt.model)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.</span>model (opts)](#apidoc.element.scuttlebutt.model.model)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.</span>super_ (opts)](#apidoc.element.scuttlebutt.model.super_)

#### [module scuttlebutt.model.prototype](#apidoc.module.scuttlebutt.model.prototype)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>applyUpdate (update)](#apidoc.element.scuttlebutt.model.prototype.applyUpdate)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>each (iter)](#apidoc.element.scuttlebutt.model.prototype.each)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>forEach (iter)](#apidoc.element.scuttlebutt.model.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>get (k)](#apidoc.element.scuttlebutt.model.prototype.get)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>history (sources)](#apidoc.element.scuttlebutt.model.prototype.history)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>keys ()](#apidoc.element.scuttlebutt.model.prototype.keys)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>set (k, v)](#apidoc.element.scuttlebutt.model.prototype.set)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>toJSON ()](#apidoc.element.scuttlebutt.model.prototype.toJSON)

#### [module scuttlebutt.util](#apidoc.module.scuttlebutt.util)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.util.</span>createId ()](#apidoc.element.scuttlebutt.util.createId)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.util.</span>filter (update, sources)](#apidoc.element.scuttlebutt.util.filter)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.util.</span>protoIsIllegal (s)](#apidoc.element.scuttlebutt.util.protoIsIllegal)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.util.</span>sort (hist)](#apidoc.element.scuttlebutt.util.sort)
1.  [function <span class="apidocSignatureSpan">scuttlebutt.util.</span>validUpdate (t, update)](#apidoc.element.scuttlebutt.util.validUpdate)



# <a name="apidoc.module.scuttlebutt"></a>[module scuttlebutt](#apidoc.module.scuttlebutt)

#### <a name="apidoc.element.scuttlebutt.events"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>events (opts)](#apidoc.element.scuttlebutt.events)
- description and source-code
```javascript
function ReliableEventEmitter(opts) {
  if(!(this instanceof ReliableEventEmitter)) return new ReliableEventEmitter(opts)
  Scuttlebutt.call(this, opts)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.filter"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>filter (update, sources)](#apidoc.element.scuttlebutt.filter)
- description and source-code
```javascript
filter = function (update, sources) {
  var ts = update[1]
  var source = update[2]
  return (!sources || !sources[source] || sources[source] < ts)
}
```
- example usage
```shell
...
outer.on('sync', function () {
  process.nextTick(function () {
    d._end()
  })
})
  }
  function onUpdate (update) { //value, source, ts
if(!validate(update) || !u.filter(update, sources))
  return

d._data(update)

//really, this should happen before emitting.
var ts = update[1]
var source = update[2]
...
```

#### <a name="apidoc.element.scuttlebutt.model"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>model (opts)](#apidoc.element.scuttlebutt.model)
- description and source-code
```javascript
function Model(opts) {
  if(!(this instanceof Model)) return new Model(opts)
  Scuttlebutt.call(this, opts)
  this.store = {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.super_"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>super_ ()](#apidoc.element.scuttlebutt.super_)
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

#### <a name="apidoc.element.scuttlebutt.timestamp"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>timestamp ()](#apidoc.element.scuttlebutt.timestamp)
- description and source-code
```javascript
function timestamp() {
<span class="apidocCodeCommentSpan">  /**
  Returns NOT an accurate representation of the current time.
  Since js only measures time as ms, if you call 'Date.now()'
  twice quickly, it's possible to get two identical time stamps.
  This function guarantees unique but maybe inaccurate results
  on each call.
  **/
</span>  //uncomment this wen
  var time = Date.now()
  //time = ~~ (time / 1000)
  //^^^uncomment when testing...

  /**
  If time returned is same as in last call, adjust it by
  adding a number based on the counter.
  Counter is incremented so that next call get's adjusted properly.
  Because floats have restricted precision,
  may need to step past some values...
  **/
  if (_last === time)  {
    do {
      adjusted = time + ((_count++) / (_count + 999))
    } while (adjusted === _adjusted)
    _adjusted = adjusted
  }
  // If last time was different reset timer back to '1'.
  else {
    _count = 1
    adjusted = time
  }
  _adjusted = adjusted
  _last = time
  return adjusted
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.updateIsRecent"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>updateIsRecent (update, sources)](#apidoc.element.scuttlebutt.updateIsRecent)
- description and source-code
```javascript
updateIsRecent = function (update, sources) {
  var ts = update[1]
  var source = update[2]
  return (!sources || !sources[source] || sources[source] < ts)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.scuttlebutt.events"></a>[module scuttlebutt.events](#apidoc.module.scuttlebutt.events)

#### <a name="apidoc.element.scuttlebutt.events.events"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>events (opts)](#apidoc.element.scuttlebutt.events.events)
- description and source-code
```javascript
function ReliableEventEmitter(opts) {
  if(!(this instanceof ReliableEventEmitter)) return new ReliableEventEmitter(opts)
  Scuttlebutt.call(this, opts)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.events.super_"></a>[function <span class="apidocSignatureSpan">scuttlebutt.events.</span>super_ (opts)](#apidoc.element.scuttlebutt.events.super_)
- description and source-code
```javascript
function Scuttlebutt(opts) {

  if(!(this instanceof Scuttlebutt)) return new Scuttlebutt(opts)
  var id = 'string' === typeof opts ? opts : opts && opts.id
  this.sources = {}
  this.setMaxListeners(Number.MAX_VALUE)
  //count how many other instances we are replicating to.
  this._streams = 0
  if(opts && opts.sign && opts.verify) {
    this.setId(opts.id || opts.createId())
    this._sign   = opts.sign
    this._verify = opts.verify
  } else {
    this.setId(id || u.createId())
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.scuttlebutt.events.prototype"></a>[module scuttlebutt.events.prototype](#apidoc.module.scuttlebutt.events.prototype)

#### <a name="apidoc.element.scuttlebutt.events.prototype.applyUpdate"></a>[function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>applyUpdate (update)](#apidoc.element.scuttlebutt.events.prototype.applyUpdate)
- description and source-code
```javascript
applyUpdate = function (update) {
  var key = update[0][0]
  this.events = this.events || {}
  this.events[key] = this.events[key] || []
  this.events[key].push(update)
  //emit the event.
  emit.apply(this, update[0])
  return true
}
```
- example usage
```shell
...

  if(err)
    return emit.call(self, 'error', err)

  if(!verified)
    return emit.call(self, 'unverified_data', update)

  if(self.applyUpdate(update))
    emit.call(self, '_update', update) //write to stream.
}

if(source !== this.id) {
  if(this._verify)
    this._verify(update, didVerification)
  else
...
```

#### <a name="apidoc.element.scuttlebutt.events.prototype.emit"></a>[function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>emit (event)](#apidoc.element.scuttlebutt.events.prototype.emit)
- description and source-code
```javascript
emit = function (event) {
  if(event === '__proto__')
    throw new Error('__proto__ is illegal event name')
  var args = [].slice.call(arguments)
  if(event == 'newListener')
    return emit.apply(this, args)
  return this.localUpdate(args)
}
```
- example usage
```shell
...
  var tail = opts.tail !== false //default to tail=true

  function start (data) {
//when the digest is recieved from the other end,
//send the history.
//merge with the current list of sources.
if (!data || !data.clock) {
    d.emit('error');
    return d._end()
}

sources = data.clock

i.each(self.history(sources), function (data) {d._data(data)})
...
```

#### <a name="apidoc.element.scuttlebutt.events.prototype.history"></a>[function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>history (filter)](#apidoc.element.scuttlebutt.events.prototype.history)
- description and source-code
```javascript
history = function (filter) {
  var self = this
  var h = []
  this.events = this.events || {}
  each(this.events, function (es) {
    each(es, function (e) {
      if(u.filter(e, filter))
        h.push(e)
    })
  })
  return u.sort(h)
}
```
- example usage
```shell
...
if (!data || !data.clock) {
    d.emit('error');
    return d._end()
}

sources = data.clock

i.each(self.history(sources), function (data) {d._data(data)})

//the _update listener must be set after the history is queued.
//otherwise there is a race between the first client message
//and the next update (which may come in on another stream)
//this problem will probably not be encountered until you have
//thousands of scuttlebutts.
...
```

#### <a name="apidoc.element.scuttlebutt.events.prototype.on"></a>[function <span class="apidocSignatureSpan">scuttlebutt.events.prototype.</span>on (event, listener)](#apidoc.element.scuttlebutt.events.prototype.on)
- description and source-code
```javascript
on = function (event, listener) {
  if(event === '__proto__')
    throw new Error('__proto__ is invalid event')
  return on.call(this, event, listener)
}
```
- example usage
```shell
...

** Any stream that gets parsed should have an error listener! **

''' js
net.createServer(function (stream) {
  var ms = m.createStream()
  stream.pipe(ms).pipe(stream)
  ms.on('error', function () {
    stream.destroy()
  })
  stream.on('error', function () {
    ms.destroy()
  })
}).listen(9999)
'''
...
```



# <a name="apidoc.module.scuttlebutt.model"></a>[module scuttlebutt.model](#apidoc.module.scuttlebutt.model)

#### <a name="apidoc.element.scuttlebutt.model.model"></a>[function <span class="apidocSignatureSpan">scuttlebutt.</span>model (opts)](#apidoc.element.scuttlebutt.model.model)
- description and source-code
```javascript
function Model(opts) {
  if(!(this instanceof Model)) return new Model(opts)
  Scuttlebutt.call(this, opts)
  this.store = {}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.model.super_"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.</span>super_ (opts)](#apidoc.element.scuttlebutt.model.super_)
- description and source-code
```javascript
function Scuttlebutt(opts) {

  if(!(this instanceof Scuttlebutt)) return new Scuttlebutt(opts)
  var id = 'string' === typeof opts ? opts : opts && opts.id
  this.sources = {}
  this.setMaxListeners(Number.MAX_VALUE)
  //count how many other instances we are replicating to.
  this._streams = 0
  if(opts && opts.sign && opts.verify) {
    this.setId(opts.id || opts.createId())
    this._sign   = opts.sign
    this._verify = opts.verify
  } else {
    this.setId(id || u.createId())
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.scuttlebutt.model.prototype"></a>[module scuttlebutt.model.prototype](#apidoc.module.scuttlebutt.model.prototype)

#### <a name="apidoc.element.scuttlebutt.model.prototype.applyUpdate"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>applyUpdate (update)](#apidoc.element.scuttlebutt.model.prototype.applyUpdate)
- description and source-code
```javascript
applyUpdate = function (update) {
  var key = update[0][0]
  if('__proto__' === key) return u.protoIsIllegal(this)
  //ignore if we already have a more recent value

  if('undefined' !== typeof this.store[key]
    && this.store[key][1] > update[1])
    return this.emit('_remove', update)

  if(this.store[key]) this.emit('_remove', this.store[key])

  this.store[key] = update

  this.emit.apply(this, ['update'].concat(update))
  this.emit('change', key, update[0][1])
  this.emit('change:'+key, update[0][1])

  return true
}
```
- example usage
```shell
...

  if(err)
    return emit.call(self, 'error', err)

  if(!verified)
    return emit.call(self, 'unverified_data', update)

  if(self.applyUpdate(update))
    emit.call(self, '_update', update) //write to stream.
}

if(source !== this.id) {
  if(this._verify)
    this._verify(update, didVerification)
  else
...
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.each"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>each (iter)](#apidoc.element.scuttlebutt.model.prototype.each)
- description and source-code
```javascript
each = function (iter) {
  for (var k in this.store)
    iter(this.store[k][0][1], k, this.store)
  return this
}
```
- example usage
```shell
...
if (!data || !data.clock) {
    d.emit('error');
    return d._end()
}

sources = data.clock

i.each(self.history(sources), function (data) {d._data(data)})

//the _update listener must be set after the history is queued.
//otherwise there is a race between the first client message
//and the next update (which may come in on another stream)
//this problem will probably not be encountered until you have
//thousands of scuttlebutts.
...
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.forEach"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>forEach (iter)](#apidoc.element.scuttlebutt.model.prototype.forEach)
- description and source-code
```javascript
forEach = function (iter) {
  for (var k in this.store)
    iter(this.store[k][0][1], k, this.store)
  return this
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.get"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>get (k)](#apidoc.element.scuttlebutt.model.prototype.get)
- description and source-code
```javascript
get = function (k) {
  if(k==='__proto__') return u.protoIsIllegal(this)
  if(this.store[k])
    return this.store[k][0][1]
}
```
- example usage
```shell
...
  })
  return u.sort(h)
}

m.toJSON = function () {
  var o = {}, notNull = false
  for (var k in this.store) {
    var v = this.get(k)
    if(v != null)
      o[k] = this.get(k)
  }
  return o
}
...
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.history"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>history (sources)](#apidoc.element.scuttlebutt.model.prototype.history)
- description and source-code
```javascript
history = function (sources) {
  var self = this
  var h = []
  each(this.store, function (e) {
    if(u.filter(e, sources))
      h.push(e)
  })
  return u.sort(h)
}
```
- example usage
```shell
...
if (!data || !data.clock) {
    d.emit('error');
    return d._end()
}

sources = data.clock

i.each(self.history(sources), function (data) {d._data(data)})

//the _update listener must be set after the history is queued.
//otherwise there is a race between the first client message
//and the next update (which may come in on another stream)
//this problem will probably not be encountered until you have
//thousands of scuttlebutts.
...
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.keys"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>keys ()](#apidoc.element.scuttlebutt.model.prototype.keys)
- description and source-code
```javascript
keys = function () {
  var a = []
  for (var k in this.store)
    a.push(k)
  return a
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.set"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>set (k, v)](#apidoc.element.scuttlebutt.model.prototype.set)
- description and source-code
```javascript
set = function (k, v) {
  if(k==='__proto__') return u.protoIsIllegal(this)
  this.localUpdate([k, v])
  return this
}
```
- example usage
```shell
...

''' js
var Model = require('scuttlebutt/model')

var a = new Model()
var b = new Model()

a.set(key, value)

b.on('update', console.log)

var s = a.createStream()
s.pipe(b.createStream()).pipe(s)
'''
...
```

#### <a name="apidoc.element.scuttlebutt.model.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">scuttlebutt.model.prototype.</span>toJSON ()](#apidoc.element.scuttlebutt.model.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  var o = {}, notNull = false
  for (var k in this.store) {
    var v = this.get(k)
    if(v != null)
      o[k] = this.get(k)
  }
  return o
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.scuttlebutt.util"></a>[module scuttlebutt.util](#apidoc.module.scuttlebutt.util)

#### <a name="apidoc.element.scuttlebutt.util.createId"></a>[function <span class="apidocSignatureSpan">scuttlebutt.util.</span>createId ()](#apidoc.element.scuttlebutt.util.createId)
- description and source-code
```javascript
createId = function () {
  return [1,1,1].map(function () {
    return Math.random().toString(16).substring(2).toUpperCase()
  }).join('')
}
```
- example usage
```shell
...
  if(!(this instanceof Scuttlebutt)) return new Scuttlebutt(opts)
  var id = 'string' === typeof opts ? opts : opts && opts.id
  this.sources = {}
  this.setMaxListeners(Number.MAX_VALUE)
  //count how many other instances we are replicating to.
  this._streams = 0
  if(opts && opts.sign && opts.verify) {
    this.setId(opts.id || opts.createId())
    this._sign   = opts.sign
    this._verify = opts.verify
  } else {
    this.setId(id || u.createId())
  }
}
...
```

#### <a name="apidoc.element.scuttlebutt.util.filter"></a>[function <span class="apidocSignatureSpan">scuttlebutt.util.</span>filter (update, sources)](#apidoc.element.scuttlebutt.util.filter)
- description and source-code
```javascript
filter = function (update, sources) {
  var ts = update[1]
  var source = update[2]
  return (!sources || !sources[source] || sources[source] < ts)
}
```
- example usage
```shell
...
outer.on('sync', function () {
  process.nextTick(function () {
    d._end()
  })
})
  }
  function onUpdate (update) { //value, source, ts
if(!validate(update) || !u.filter(update, sources))
  return

d._data(update)

//really, this should happen before emitting.
var ts = update[1]
var source = update[2]
...
```

#### <a name="apidoc.element.scuttlebutt.util.protoIsIllegal"></a>[function <span class="apidocSignatureSpan">scuttlebutt.util.</span>protoIsIllegal (s)](#apidoc.element.scuttlebutt.util.protoIsIllegal)
- description and source-code
```javascript
protoIsIllegal = function (s) {
  s.emit('invalid', new Error('"__proto__" is illegal property name'))
  return null
}
```
- example usage
```shell
...
Scuttlebutt.call(this, opts)
this.store = {}
}

var m = Model.prototype

m.set = function (k, v) {
if(k==='__proto__') return u.protoIsIllegal(this)
this.localUpdate([k, v])
return this
}


m.get = function (k) {
if(k==='__proto__') return u.protoIsIllegal(this)
...
```

#### <a name="apidoc.element.scuttlebutt.util.sort"></a>[function <span class="apidocSignatureSpan">scuttlebutt.util.</span>sort (hist)](#apidoc.element.scuttlebutt.util.sort)
- description and source-code
```javascript
sort = function (hist) {
  return hist.sort(function (a, b) {
    //sort by timestamps, then ids.
    //there should never be a pair with equal timestamps
    //and ids.
    return a[1] - b[1] || (a[2] > b[2] ? 1 : -1)
  })
}
```
- example usage
```shell
...
  this.events = this.events || {}
  each(this.events, function (es) {
    each(es, function (e) {
      if(u.filter(e, filter))
        h.push(e)
    })
  })
  return u.sort(h)
}
...
```

#### <a name="apidoc.element.scuttlebutt.util.validUpdate"></a>[function <span class="apidocSignatureSpan">scuttlebutt.util.</span>validUpdate (t, update)](#apidoc.element.scuttlebutt.util.validUpdate)
- description and source-code
```javascript
validUpdate = function (t, update) {
  if(!Array.isArray(update)) return invalidUpdate(t)
  if('string' !== typeof update[1] || 'number' !== typeof update[2])
    return invalidUpdate(t)
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
