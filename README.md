# api documentation for  [consul (v0.28.0)](https://github.com/silas/node-consul#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-consul.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-consul) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-consul.svg)](https://travis-ci.org/npmdoc/node-npmdoc-consul)
#### Consul client

[![NPM](https://nodei.co/npm/consul.png?downloads=true)](https://www.npmjs.com/package/consul)

[![apidoc](https://npmdoc.github.io/node-npmdoc-consul/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-consul_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-consul/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-consul/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-consul/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Silas Sewell",
        "email": "silas@sewell.org"
    },
    "bugs": {
        "url": "https://github.com/silas/node-consul/issues"
    },
    "dependencies": {
        "papi": "^0.27.0"
    },
    "description": "Consul client",
    "devDependencies": {
        "async": "^1.4.0",
        "bluebird": "^3.1.1",
        "debug": "^2.1.3",
        "istanbul": "^0.3.8",
        "jscs": "^2.1.1",
        "jshint": "^2.5.5",
        "lodash": "^3.5.0",
        "mocha": "^2.2.1",
        "nock": "^2.9.1",
        "node-uuid": "^1.4.3",
        "should": "^7.0.2",
        "sinon": "^1.14.1",
        "temp": "^0.8.1"
    },
    "directories": {},
    "dist": {
        "shasum": "c478fe6c58b6154b72867ef57ca8cfac181fba92",
        "tarball": "https://registry.npmjs.org/consul/-/consul-0.28.0.tgz"
    },
    "gitHead": "a0726641a976a8c93bac67754a764bc90642eab3",
    "homepage": "https://github.com/silas/node-consul#readme",
    "keywords": [
        "consul"
    ],
    "license": "MIT",
    "main": "./lib",
    "maintainers": [
        {
            "name": "silas",
            "email": "silas@sewell.org"
        }
    ],
    "name": "consul",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/silas/node-consul.git"
    },
    "scripts": {
        "acceptance": "ACCEPTANCE=true istanbul cover --report text _mocha -- test/acceptance --recursive --check-leaks --timeout 15000",
        "cover": "istanbul cover _mocha -- --recursive && open coverage/lcov-report/index.html",
        "test": "jshint lib test && jscs lib test && istanbul cover --report text _mocha -- --recursive --check-leaks && istanbul check-coverage --statements 100 --functions 100 --branches 100 --lines 100"
    },
    "version": "0.28.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module consul](#apidoc.module.consul)
1.  [function <span class="apidocSignatureSpan">consul.</span>Acl (consul)](#apidoc.element.consul.Acl)
1.  [function <span class="apidocSignatureSpan">consul.</span>Agent (consul)](#apidoc.element.consul.Agent)
1.  [function <span class="apidocSignatureSpan">consul.</span>Agent.Check (consul)](#apidoc.element.consul.Agent.Check)
1.  [function <span class="apidocSignatureSpan">consul.</span>Agent.Service (consul)](#apidoc.element.consul.Agent.Service)
1.  [function <span class="apidocSignatureSpan">consul.</span>Catalog (consul)](#apidoc.element.consul.Catalog)
1.  [function <span class="apidocSignatureSpan">consul.</span>Catalog.Node (consul)](#apidoc.element.consul.Catalog.Node)
1.  [function <span class="apidocSignatureSpan">consul.</span>Catalog.Service (consul)](#apidoc.element.consul.Catalog.Service)
1.  [function <span class="apidocSignatureSpan">consul.</span>Event (consul)](#apidoc.element.consul.Event)
1.  [function <span class="apidocSignatureSpan">consul.</span>Health (consul)](#apidoc.element.consul.Health)
1.  [function <span class="apidocSignatureSpan">consul.</span>Kv (consul)](#apidoc.element.consul.Kv)
1.  [function <span class="apidocSignatureSpan">consul.</span>Lock (consul, opts)](#apidoc.element.consul.Lock)
1.  [function <span class="apidocSignatureSpan">consul.</span>Query (consul)](#apidoc.element.consul.Query)
1.  [function <span class="apidocSignatureSpan">consul.</span>Session (consul)](#apidoc.element.consul.Session)
1.  [function <span class="apidocSignatureSpan">consul.</span>Status (consul)](#apidoc.element.consul.Status)
1.  [function <span class="apidocSignatureSpan">consul.</span>Watch (consul, opts)](#apidoc.element.consul.Watch)
1.  [function <span class="apidocSignatureSpan">consul.</span>parseQueryMeta (res)](#apidoc.element.consul.parseQueryMeta)
1.  [function <span class="apidocSignatureSpan">consul.</span>super_ (opts)](#apidoc.element.consul.super_)
1.  [function <span class="apidocSignatureSpan">consul.</span>walk ()](#apidoc.element.consul.walk)
1.  object <span class="apidocSignatureSpan"></span>consul
1.  object <span class="apidocSignatureSpan">consul.</span>Acl.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Agent.Check.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Agent.Service.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Agent.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Catalog.Node.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Catalog.Service.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Catalog.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Event.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Health.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Kv.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Lock.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Query.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Session.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Status.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>Watch.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>acl
1.  object <span class="apidocSignatureSpan">consul.</span>agent
1.  object <span class="apidocSignatureSpan">consul.</span>catalog
1.  object <span class="apidocSignatureSpan">consul.</span>errors
1.  object <span class="apidocSignatureSpan">consul.</span>event
1.  object <span class="apidocSignatureSpan">consul.</span>health
1.  object <span class="apidocSignatureSpan">consul.</span>kv
1.  object <span class="apidocSignatureSpan">consul.</span>lock
1.  object <span class="apidocSignatureSpan">consul.</span>meta
1.  object <span class="apidocSignatureSpan">consul.</span>query
1.  object <span class="apidocSignatureSpan">consul.</span>session
1.  object <span class="apidocSignatureSpan">consul.</span>status
1.  object <span class="apidocSignatureSpan">consul.</span>super_.prototype
1.  object <span class="apidocSignatureSpan">consul.</span>utils
1.  object <span class="apidocSignatureSpan">consul.</span>watch

#### [module consul.Acl](#apidoc.module.consul.Acl)
1.  [function <span class="apidocSignatureSpan">consul.</span>Acl (consul)](#apidoc.element.consul.Acl.Acl)

#### [module consul.Acl.prototype](#apidoc.module.consul.Acl.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>clone (opts, callback)](#apidoc.element.consul.Acl.prototype.clone)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>create (opts, callback)](#apidoc.element.consul.Acl.prototype.create)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>destroy (opts, callback)](#apidoc.element.consul.Acl.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>get (opts, callback)](#apidoc.element.consul.Acl.prototype.get)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>info (opts, callback)](#apidoc.element.consul.Acl.prototype.info)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>list (opts, callback)](#apidoc.element.consul.Acl.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>update (opts, callback)](#apidoc.element.consul.Acl.prototype.update)

#### [module consul.Agent](#apidoc.module.consul.Agent)
1.  [function <span class="apidocSignatureSpan">consul.</span>Agent (consul)](#apidoc.element.consul.Agent.Agent)
1.  [function <span class="apidocSignatureSpan">consul.Agent.</span>Check (consul)](#apidoc.element.consul.Agent.Check)
1.  [function <span class="apidocSignatureSpan">consul.Agent.</span>Service (consul)](#apidoc.element.consul.Agent.Service)

#### [module consul.Agent.Check](#apidoc.module.consul.Agent.Check)
1.  [function <span class="apidocSignatureSpan">consul.Agent.</span>Check (consul)](#apidoc.element.consul.Agent.Check.Check)

#### [module consul.Agent.Check.prototype](#apidoc.module.consul.Agent.Check.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>deregister (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.deregister)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>fail (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.fail)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>list (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>pass (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.pass)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>register (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.register)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>warn (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.warn)

#### [module consul.Agent.Service](#apidoc.module.consul.Agent.Service)
1.  [function <span class="apidocSignatureSpan">consul.Agent.</span>Service (consul)](#apidoc.element.consul.Agent.Service.Service)

#### [module consul.Agent.Service.prototype](#apidoc.module.consul.Agent.Service.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>deregister (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.deregister)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>list (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>maintenance (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.maintenance)
1.  [function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>register (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.register)

#### [module consul.Agent.prototype](#apidoc.module.consul.Agent.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>checks ()](#apidoc.element.consul.Agent.prototype.checks)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>forceLeave (opts, callback)](#apidoc.element.consul.Agent.prototype.forceLeave)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>join (opts, callback)](#apidoc.element.consul.Agent.prototype.join)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>maintenance (opts, callback)](#apidoc.element.consul.Agent.prototype.maintenance)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>members (opts, callback)](#apidoc.element.consul.Agent.prototype.members)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>self (opts, callback)](#apidoc.element.consul.Agent.prototype.self)
1.  [function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>services ()](#apidoc.element.consul.Agent.prototype.services)

#### [module consul.Catalog](#apidoc.module.consul.Catalog)
1.  [function <span class="apidocSignatureSpan">consul.</span>Catalog (consul)](#apidoc.element.consul.Catalog.Catalog)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.</span>Node (consul)](#apidoc.element.consul.Catalog.Node)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.</span>Service (consul)](#apidoc.element.consul.Catalog.Service)

#### [module consul.Catalog.Node](#apidoc.module.consul.Catalog.Node)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.</span>Node (consul)](#apidoc.element.consul.Catalog.Node.Node)

#### [module consul.Catalog.Node.prototype](#apidoc.module.consul.Catalog.Node.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.Node.prototype.</span>list (opts, callback)](#apidoc.element.consul.Catalog.Node.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.Node.prototype.</span>services (opts, callback)](#apidoc.element.consul.Catalog.Node.prototype.services)

#### [module consul.Catalog.Service](#apidoc.module.consul.Catalog.Service)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.</span>Service (consul)](#apidoc.element.consul.Catalog.Service.Service)

#### [module consul.Catalog.Service.prototype](#apidoc.module.consul.Catalog.Service.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.Service.prototype.</span>list (opts, callback)](#apidoc.element.consul.Catalog.Service.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.Service.prototype.</span>nodes (opts, callback)](#apidoc.element.consul.Catalog.Service.prototype.nodes)

#### [module consul.Catalog.prototype](#apidoc.module.consul.Catalog.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.prototype.</span>datacenters (opts, callback)](#apidoc.element.consul.Catalog.prototype.datacenters)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.prototype.</span>nodes ()](#apidoc.element.consul.Catalog.prototype.nodes)
1.  [function <span class="apidocSignatureSpan">consul.Catalog.prototype.</span>services ()](#apidoc.element.consul.Catalog.prototype.services)

#### [module consul.Event](#apidoc.module.consul.Event)
1.  [function <span class="apidocSignatureSpan">consul.</span>Event (consul)](#apidoc.element.consul.Event.Event)

#### [module consul.Event.prototype](#apidoc.module.consul.Event.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Event.prototype.</span>fire (opts, callback)](#apidoc.element.consul.Event.prototype.fire)
1.  [function <span class="apidocSignatureSpan">consul.Event.prototype.</span>list (opts, callback)](#apidoc.element.consul.Event.prototype.list)

#### [module consul.Health](#apidoc.module.consul.Health)
1.  [function <span class="apidocSignatureSpan">consul.</span>Health (consul)](#apidoc.element.consul.Health.Health)

#### [module consul.Health.prototype](#apidoc.module.consul.Health.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Health.prototype.</span>checks (opts, callback)](#apidoc.element.consul.Health.prototype.checks)
1.  [function <span class="apidocSignatureSpan">consul.Health.prototype.</span>node (opts, callback)](#apidoc.element.consul.Health.prototype.node)
1.  [function <span class="apidocSignatureSpan">consul.Health.prototype.</span>service (opts, callback)](#apidoc.element.consul.Health.prototype.service)
1.  [function <span class="apidocSignatureSpan">consul.Health.prototype.</span>state (opts, callback)](#apidoc.element.consul.Health.prototype.state)

#### [module consul.Kv](#apidoc.module.consul.Kv)
1.  [function <span class="apidocSignatureSpan">consul.</span>Kv (consul)](#apidoc.element.consul.Kv.Kv)
1.  object <span class="apidocSignatureSpan">consul.Kv.</span>meta

#### [module consul.Kv.prototype](#apidoc.module.consul.Kv.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>del (opts, callback)](#apidoc.element.consul.Kv.prototype.del)
1.  [function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>delete (opts, callback)](#apidoc.element.consul.Kv.prototype.delete)
1.  [function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>get (opts, callback)](#apidoc.element.consul.Kv.prototype.get)
1.  [function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>keys (opts, callback)](#apidoc.element.consul.Kv.prototype.keys)
1.  [function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>set (opts, callback)](#apidoc.element.consul.Kv.prototype.set)

#### [module consul.Lock](#apidoc.module.consul.Lock)
1.  [function <span class="apidocSignatureSpan">consul.</span>Lock (consul, opts)](#apidoc.element.consul.Lock.Lock)
1.  [function <span class="apidocSignatureSpan">consul.Lock.</span>super_ ()](#apidoc.element.consul.Lock.super_)
1.  object <span class="apidocSignatureSpan">consul.Lock.</span>meta

#### [module consul.Lock.prototype](#apidoc.module.consul.Lock.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_acquire (ctx)](#apidoc.element.consul.Lock.prototype._acquire)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_end (ctx, err, res)](#apidoc.element.consul.Lock.prototype._end)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_err (err, res)](#apidoc.element.consul.Lock.prototype._err)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_monitor (ctx)](#apidoc.element.consul.Lock.prototype._monitor)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_release (ctx)](#apidoc.element.consul.Lock.prototype._release)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_run (ctx)](#apidoc.element.consul.Lock.prototype._run)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_session (ctx)](#apidoc.element.consul.Lock.prototype._session)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_wait (ctx)](#apidoc.element.consul.Lock.prototype._wait)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>acquire ()](#apidoc.element.consul.Lock.prototype.acquire)
1.  [function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>release ()](#apidoc.element.consul.Lock.prototype.release)

#### [module consul.Query](#apidoc.module.consul.Query)
1.  [function <span class="apidocSignatureSpan">consul.</span>Query (consul)](#apidoc.element.consul.Query.Query)

#### [module consul.Query.prototype](#apidoc.module.consul.Query.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>_params (req, opts)](#apidoc.element.consul.Query.prototype._params)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>create (opts, callback)](#apidoc.element.consul.Query.prototype.create)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>destroy (opts, callback)](#apidoc.element.consul.Query.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>execute (opts, callback)](#apidoc.element.consul.Query.prototype.execute)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>explain (opts, callback)](#apidoc.element.consul.Query.prototype.explain)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>get (opts, callback)](#apidoc.element.consul.Query.prototype.get)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>list (opts, callback)](#apidoc.element.consul.Query.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Query.prototype.</span>update (opts, callback)](#apidoc.element.consul.Query.prototype.update)

#### [module consul.Session](#apidoc.module.consul.Session)
1.  [function <span class="apidocSignatureSpan">consul.</span>Session (consul)](#apidoc.element.consul.Session.Session)

#### [module consul.Session.prototype](#apidoc.module.consul.Session.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>create (opts, callback)](#apidoc.element.consul.Session.prototype.create)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>destroy (opts, callback)](#apidoc.element.consul.Session.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>get (opts, callback)](#apidoc.element.consul.Session.prototype.get)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>info (opts, callback)](#apidoc.element.consul.Session.prototype.info)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>list (opts, callback)](#apidoc.element.consul.Session.prototype.list)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>node (opts, callback)](#apidoc.element.consul.Session.prototype.node)
1.  [function <span class="apidocSignatureSpan">consul.Session.prototype.</span>renew (opts, callback)](#apidoc.element.consul.Session.prototype.renew)

#### [module consul.Status](#apidoc.module.consul.Status)
1.  [function <span class="apidocSignatureSpan">consul.</span>Status (consul)](#apidoc.element.consul.Status.Status)

#### [module consul.Status.prototype](#apidoc.module.consul.Status.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Status.prototype.</span>leader (opts, callback)](#apidoc.element.consul.Status.prototype.leader)
1.  [function <span class="apidocSignatureSpan">consul.Status.prototype.</span>peers (opts, callback)](#apidoc.element.consul.Status.prototype.peers)

#### [module consul.Watch](#apidoc.module.consul.Watch)
1.  [function <span class="apidocSignatureSpan">consul.</span>Watch (consul, opts)](#apidoc.element.consul.Watch.Watch)
1.  [function <span class="apidocSignatureSpan">consul.Watch.</span>super_ ()](#apidoc.element.consul.Watch.super_)
1.  object <span class="apidocSignatureSpan">consul.Watch.</span>meta

#### [module consul.Watch.prototype](#apidoc.module.consul.Watch.prototype)
1.  [function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>_err (err, res)](#apidoc.element.consul.Watch.prototype._err)
1.  [function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>_run ()](#apidoc.element.consul.Watch.prototype._run)
1.  [function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>_wait ()](#apidoc.element.consul.Watch.prototype._wait)
1.  [function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>end ()](#apidoc.element.consul.Watch.prototype.end)
1.  [function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>isRunning ()](#apidoc.element.consul.Watch.prototype.isRunning)
1.  [function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>updateTime ()](#apidoc.element.consul.Watch.prototype.updateTime)

#### [module consul.acl](#apidoc.module.consul.acl)
1.  [function <span class="apidocSignatureSpan">consul.acl.</span>Acl (consul)](#apidoc.element.consul.acl.Acl)

#### [module consul.agent](#apidoc.module.consul.agent)
1.  [function <span class="apidocSignatureSpan">consul.agent.</span>Agent (consul)](#apidoc.element.consul.agent.Agent)

#### [module consul.catalog](#apidoc.module.consul.catalog)
1.  [function <span class="apidocSignatureSpan">consul.catalog.</span>Catalog (consul)](#apidoc.element.consul.catalog.Catalog)

#### [module consul.consul](#apidoc.module.consul.consul)
1.  [function <span class="apidocSignatureSpan">consul.consul.</span>Consul (opts)](#apidoc.element.consul.consul.Consul)

#### [module consul.errors](#apidoc.module.consul.errors)
1.  [function <span class="apidocSignatureSpan">consul.errors.</span>Consul (message)](#apidoc.element.consul.errors.Consul)
1.  [function <span class="apidocSignatureSpan">consul.errors.</span>Validation (message)](#apidoc.element.consul.errors.Validation)

#### [module consul.event](#apidoc.module.consul.event)
1.  [function <span class="apidocSignatureSpan">consul.event.</span>Event (consul)](#apidoc.element.consul.event.Event)

#### [module consul.health](#apidoc.module.consul.health)
1.  [function <span class="apidocSignatureSpan">consul.health.</span>Health (consul)](#apidoc.element.consul.health.Health)

#### [module consul.kv](#apidoc.module.consul.kv)
1.  [function <span class="apidocSignatureSpan">consul.kv.</span>Kv (consul)](#apidoc.element.consul.kv.Kv)

#### [module consul.lock](#apidoc.module.consul.lock)
1.  [function <span class="apidocSignatureSpan">consul.lock.</span>Lock (consul, opts)](#apidoc.element.consul.lock.Lock)

#### [module consul.query](#apidoc.module.consul.query)
1.  [function <span class="apidocSignatureSpan">consul.query.</span>Query (consul)](#apidoc.element.consul.query.Query)

#### [module consul.session](#apidoc.module.consul.session)
1.  [function <span class="apidocSignatureSpan">consul.session.</span>Session (consul)](#apidoc.element.consul.session.Session)

#### [module consul.status](#apidoc.module.consul.status)
1.  [function <span class="apidocSignatureSpan">consul.status.</span>Status (consul)](#apidoc.element.consul.status.Status)

#### [module consul.super_](#apidoc.module.consul.super_)
1.  [function <span class="apidocSignatureSpan">consul.</span>super_ ()](#apidoc.element.consul.super_.super_)

#### [module consul.super_.prototype](#apidoc.module.consul.super_.prototype)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>__create (request, next)](#apidoc.element.consul.super_.prototype.__create)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>__execute (request, next)](#apidoc.element.consul.super_.prototype.__execute)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>__push (request, name)](#apidoc.element.consul.super_.prototype.__push)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_decode (mime, value)](#apidoc.element.consul.super_.prototype._decode)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_delete (opts)](#apidoc.element.consul.super_.prototype._delete)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_encode (mime, value)](#apidoc.element.consul.super_.prototype._encode)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_err (err, opts)](#apidoc.element.consul.super_.prototype._err)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_ext (eventName, callback)](#apidoc.element.consul.super_.prototype._ext)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_get (opts)](#apidoc.element.consul.super_.prototype._get)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_head (opts)](#apidoc.element.consul.super_.prototype._head)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_log (tags, data)](#apidoc.element.consul.super_.prototype._log)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_options (opts)](#apidoc.element.consul.super_.prototype._options)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_patch (opts)](#apidoc.element.consul.super_.prototype._patch)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_plugin (plugin, options)](#apidoc.element.consul.super_.prototype._plugin)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_post (opts)](#apidoc.element.consul.super_.prototype._post)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_put (opts)](#apidoc.element.consul.super_.prototype._put)
1.  [function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_request (opts)](#apidoc.element.consul.super_.prototype._request)

#### [module consul.utils](#apidoc.module.consul.utils)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>body (request, next)](#apidoc.element.consul.utils.body)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>bodyItem (request, next)](#apidoc.element.consul.utils.bodyItem)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>clone (src)](#apidoc.element.consul.utils.clone)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>createCheck (src)](#apidoc.element.consul.utils.createCheck)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>createServiceCheck (src)](#apidoc.element.consul.utils.createServiceCheck)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>decode (value, opts)](#apidoc.element.consul.utils.decode)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>defaults (obj)](#apidoc.element.consul.utils.defaults)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>empty (request, next)](#apidoc.element.consul.utils.empty)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>hasIndexChanged (index, prevIndex)](#apidoc.element.consul.utils.hasIndexChanged)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>normalizeKeys (obj)](#apidoc.element.consul.utils.normalizeKeys)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>options (req, opts)](#apidoc.element.consul.utils.options)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>parseDuration (value)](#apidoc.element.consul.utils.parseDuration)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>parseQueryMeta (res)](#apidoc.element.consul.utils.parseQueryMeta)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>setIntervalContext (fn, ctx, timeout)](#apidoc.element.consul.utils.setIntervalContext)
1.  [function <span class="apidocSignatureSpan">consul.utils.</span>setTimeoutContext (fn, ctx, timeout)](#apidoc.element.consul.utils.setTimeoutContext)

#### [module consul.watch](#apidoc.module.consul.watch)
1.  [function <span class="apidocSignatureSpan">consul.watch.</span>Watch (consul, opts)](#apidoc.element.consul.watch.Watch)



# <a name="apidoc.module.consul"></a>[module consul](#apidoc.module.consul)

#### <a name="apidoc.element.consul.Acl"></a>[function <span class="apidocSignatureSpan">consul.</span>Acl (consul)](#apidoc.element.consul.Acl)
- description and source-code
```javascript
function Acl(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

  if (defaults) this._defaults = defaults;
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
...
```

#### <a name="apidoc.element.consul.Agent"></a>[function <span class="apidocSignatureSpan">consul.</span>Agent (consul)](#apidoc.element.consul.Agent)
- description and source-code
```javascript
function Agent(consul) {
  this.consul = consul;
  this.check = new Agent.Check(consul);
  this.service = new Agent.Service(consul);
}
```
- example usage
```shell
...
  if (defaults) this._defaults = defaults;
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);
...
```

#### <a name="apidoc.element.consul.Agent.Check"></a>[function <span class="apidocSignatureSpan">consul.</span>Agent.Check (consul)](#apidoc.element.consul.Agent.Check)
- description and source-code
```javascript
function AgentCheck(consul) {
  this.consul = consul;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Agent.Service"></a>[function <span class="apidocSignatureSpan">consul.</span>Agent.Service (consul)](#apidoc.element.consul.Agent.Service)
- description and source-code
```javascript
function AgentService(consul) {
  this.consul = consul;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Catalog"></a>[function <span class="apidocSignatureSpan">consul.</span>Catalog (consul)](#apidoc.element.consul.Catalog)
- description and source-code
```javascript
function Catalog(consul) {
  this.consul = consul;
  this.node = new Catalog.Node(consul);
  this.service = new Catalog.Service(consul);
}
```
- example usage
```shell
...
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);
...
```

#### <a name="apidoc.element.consul.Catalog.Node"></a>[function <span class="apidocSignatureSpan">consul.</span>Catalog.Node (consul)](#apidoc.element.consul.Catalog.Node)
- description and source-code
```javascript
function CatalogNode(consul) {
  this.consul = consul;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Catalog.Service"></a>[function <span class="apidocSignatureSpan">consul.</span>Catalog.Service (consul)](#apidoc.element.consul.Catalog.Service)
- description and source-code
```javascript
function CatalogService(consul) {
  this.consul = consul;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Event"></a>[function <span class="apidocSignatureSpan">consul.</span>Event (consul)](#apidoc.element.consul.Event)
- description and source-code
```javascript
function Event(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
...
```

#### <a name="apidoc.element.consul.Health"></a>[function <span class="apidocSignatureSpan">consul.</span>Health (consul)](#apidoc.element.consul.Health)
- description and source-code
```javascript
function Health(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
...
```

#### <a name="apidoc.element.consul.Kv"></a>[function <span class="apidocSignatureSpan">consul.</span>Kv (consul)](#apidoc.element.consul.Kv)
- description and source-code
```javascript
function Kv(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
...
```

#### <a name="apidoc.element.consul.Lock"></a>[function <span class="apidocSignatureSpan">consul.</span>Lock (consul, opts)](#apidoc.element.consul.Lock)
- description and source-code
```javascript
function Lock(consul, opts) {
  events.EventEmitter.call(this);

  opts = utils.normalizeKeys(opts);

  this.consul = consul;
  this._opts = opts;

  if (opts.session) {
    switch (typeof opts.session) {
      case 'string':
        opts.session = { id: opts.session };
        break;
      case 'object':
        opts.session = utils.normalizeKeys(opts.session);
        break;
      default:
        throw errors.Validation('session must be an object or string');
    }
  } else {
    opts.session = {};
  }

  if (!opts.key) {
    throw errors.Validation('key required');
  } else if (typeof opts.key !== 'string') {
    throw errors.Validation('key must be a string');
  }
}
```
- example usage
```shell
...
/**
 * Lock helper.
 */

Consul.meta.lock = { type: 'eventemitter' };

Consul.prototype.lock = function(opts) {
  return new Consul.Lock(this, opts);
};

/**
 * Watch helper.
 */

Consul.meta.watch = { type: 'eventemitter' };
...
```

#### <a name="apidoc.element.consul.Query"></a>[function <span class="apidocSignatureSpan">consul.</span>Query (consul)](#apidoc.element.consul.Query)
- description and source-code
```javascript
function Query(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
...
```

#### <a name="apidoc.element.consul.Session"></a>[function <span class="apidocSignatureSpan">consul.</span>Session (consul)](#apidoc.element.consul.Session)
- description and source-code
```javascript
function Session(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
    } else {
...
```

#### <a name="apidoc.element.consul.Status"></a>[function <span class="apidocSignatureSpan">consul.</span>Status (consul)](#apidoc.element.consul.Status)
- description and source-code
```javascript
function Status(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
    } else {
      papi.tools.promisify(this);
...
```

#### <a name="apidoc.element.consul.Watch"></a>[function <span class="apidocSignatureSpan">consul.</span>Watch (consul, opts)](#apidoc.element.consul.Watch)
- description and source-code
```javascript
function Watch(consul, opts) {
  var self = this;

  events.EventEmitter.call(self);

  opts = utils.normalizeKeys(opts);

  var options = utils.normalizeKeys(opts.options || {});
  options = utils.defaults(options, consul._defaults);
  options.wait = options.wait || '30s';
  options.index = options.index || '0';

  self._context = { consul: consul };
  self._options = options;
  self._attempts = 0;
  self._method = opts.method;

  if (typeof opts.method !== 'function') {
    throw errors.Validation('method required');
  }

  process.nextTick(function() { self._run(); });
}
```
- example usage
```shell
...
/**
 * Watch helper.
 */

Consul.meta.watch = { type: 'eventemitter' };

Consul.prototype.watch = function(opts) {
  return new Consul.Watch(this, opts);
};

/**
 * Walk methods
 */

Consul.meta.walk = { type: 'sync' };
...
```

#### <a name="apidoc.element.consul.parseQueryMeta"></a>[function <span class="apidocSignatureSpan">consul.</span>parseQueryMeta (res)](#apidoc.element.consul.parseQueryMeta)
- description and source-code
```javascript
parseQueryMeta = function (res) {
  return utils.parseQueryMeta(res);
}
```
- example usage
```shell
...
/**
 * Parse query meta
 */

Consul.meta.parseQueryMeta = { type: 'sync' };

Consul.parseQueryMeta = Consul.prototype.parseQueryMeta = function(res) {
  return utils.parseQueryMeta(res);
};

/**
 * Module exports.
 */

exports.Consul = Consul;
...
```

#### <a name="apidoc.element.consul.super_"></a>[function <span class="apidocSignatureSpan">consul.</span>super_ (opts)](#apidoc.element.consul.super_)
- description and source-code
```javascript
function Client(opts) {
  if (!(this instanceof Client)) {
    return new Client(opts);
  }

  events.EventEmitter.call(this);

  opts = opts || {};

  if (typeof opts === 'string') {
    opts = { baseUrl: opts };
  } else {
    opts = utils.merge(opts);
  }

  if (!opts.baseUrl) {
    throw errors.Validation('baseUrl required');
  }

  if (!(opts.baseUrl instanceof url.Url)) {
    if (typeof opts.baseUrl !== 'string') {
      throw errors.Validation('baseUrl must be a string: ' + opts.baseUrl);
    }

    opts.baseUrl = url.parse(opts.baseUrl);
  }

  var path = opts.baseUrl.pathname;
  opts.baseUrl = utils.pick(opts.baseUrl,
    'auth', 'hostname', 'port', 'protocol');
  opts.baseUrl.path = path;

  if (opts.baseUrl.path === '/') {
    opts.baseUrl.path = '';
  } else if (opts.baseUrl.path[opts.baseUrl.path.length - 1] === '/') {
    throw errors.Validation('baseUrl must not end with a forward slash');
  }

  opts.headers = utils.mergeHeaders(opts.headers);
  if (opts.tags) {
    if (Array.isArray(opts.tags)) {
      opts.tags = opts.tags.slice(0);
    } else {
      throw errors.Validation('tags must be an array');
    }
  } else {
    opts.tags = [];
  }

  if (opts.name && !~opts.tags.indexOf(opts.name)) {
    opts.tags.push(opts.name);
  }

  opts.encoders = utils.merge(constants.ENCODERS, opts.encoders);
  opts.decoders = utils.merge(constants.DECODERS, opts.decoders);

  this._opts = opts;
  this._exts = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.walk"></a>[function <span class="apidocSignatureSpan">consul.</span>walk ()](#apidoc.element.consul.walk)
- description and source-code
```javascript
walk = function () {
  return papi.tools.walk(Consul);
}
```
- example usage
```shell
...
/**
 * Walk methods
 */

Consul.meta.walk = { type: 'sync' };

Consul.walk = Consul.prototype.walk = function() {
  return papi.tools.walk(Consul);
};

/**
 * Parse query meta
 */

Consul.meta.parseQueryMeta = { type: 'sync' };
...
```



# <a name="apidoc.module.consul.Acl"></a>[module consul.Acl](#apidoc.module.consul.Acl)

#### <a name="apidoc.element.consul.Acl.Acl"></a>[function <span class="apidocSignatureSpan">consul.</span>Acl (consul)](#apidoc.element.consul.Acl.Acl)
- description and source-code
```javascript
function Acl(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

  if (defaults) this._defaults = defaults;
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
...
```



# <a name="apidoc.module.consul.Acl.prototype"></a>[module consul.Acl.prototype](#apidoc.module.consul.Acl.prototype)

#### <a name="apidoc.element.consul.Acl.prototype.clone"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>clone (opts, callback)](#apidoc.element.consul.Acl.prototype.clone)
- description and source-code
```javascript
clone = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.clone',
    path: '/acl/clone/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.body, callback);
}
```
- example usage
```shell
...
 "Name": "Read only",
 "Type": "client",
 "Rules": "{\"key\":{\"\":{\"policy\":\"read\"}}}"
}
'''

<a name="acl-clone"></a>
### consul.acl.clone(options, callback)

Creates a new token by cloning an existing token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Acl.prototype.create"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>create (opts, callback)](#apidoc.element.consul.Acl.prototype.create)
- description and source-code
```javascript
create = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.create',
    path: '/acl/create',
    query: {},
    type: 'json',
    body: {},
  };

  if (opts.name) req.body.Name = opts.name;
  if (opts.type) req.body.Type = opts.type;
  if (opts.rules) req.body.Rules = opts.rules;

  utils.options(req, opts);

  this.consul._put(req, utils.body, callback);
}
```
- example usage
```shell
...
* [update](#acl-update)
* [destroy](#acl-destroy)
* [get](#acl-get)
* [clone](#acl-clone)
* [list](#acl-list)

<a name="acl-create"></a>
### consul.acl.create([options], callback)

Creates a new token with policy.

Options

* name (String, optional): human readable name for the token
* type (String, enum: client, management; default: client): type of token
...
```

#### <a name="apidoc.element.consul.Acl.prototype.destroy"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>destroy (opts, callback)](#apidoc.element.consul.Acl.prototype.destroy)
- description and source-code
```javascript
destroy = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.destroy',
    path: '/acl/destroy/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.acl.update({ id: '63e1d82e-f718-eb92-3b7d-61f0c71d45b4', name: 'test' }, function(err) {
 if (err) throw err;
});
'''

<a name="acl-destroy"></a>
### consul.acl.destroy(options, callback)

Destroys a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Acl.prototype.get"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>get (opts, callback)](#apidoc.element.consul.Acl.prototype.get)
- description and source-code
```javascript
get = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.info',
    path: '/acl/info/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.bodyItem, callback);
}
```
- example usage
```shell
...
''' javascript
consul.acl.destroy('b1f4c10e-b61b-e1de-de95-218c9fefdd3e', function(err) {
 if (err) throw err;
});
'''

<a name="acl-get"></a>
### consul.acl.get(options, callback)

Queries the policy of a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Acl.prototype.info"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>info (opts, callback)](#apidoc.element.consul.Acl.prototype.info)
- description and source-code
```javascript
info = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.info',
    path: '/acl/info/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.bodyItem, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Acl.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>list (opts, callback)](#apidoc.element.consul.Acl.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.list',
    path: '/acl/list',
    query: {},
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Acl.prototype.update"></a>[function <span class="apidocSignatureSpan">consul.Acl.prototype.</span>update (opts, callback)](#apidoc.element.consul.Acl.prototype.update)
- description and source-code
```javascript
update = function (opts, callback) {
  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'acl.update',
    path: '/acl/update',
    query: {},
    type: 'json',
    body: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  req.body.ID = opts.id;

  if (opts.name) req.body.Name = opts.name;
  if (opts.type) req.body.Type = opts.type;
  if (opts.rules) req.body.Rules = opts.rules;

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' json
{
 "ID": "b1f4c10e-b61b-e1de-de95-218c9fefdd3e"
}
'''

<a name="acl-update"></a>
### consul.acl.update(options, callback)

Update the policy of a token.

Options

* id (String): token ID
* name (String, optional): human readable name for the token
...
```



# <a name="apidoc.module.consul.Agent"></a>[module consul.Agent](#apidoc.module.consul.Agent)

#### <a name="apidoc.element.consul.Agent.Agent"></a>[function <span class="apidocSignatureSpan">consul.</span>Agent (consul)](#apidoc.element.consul.Agent.Agent)
- description and source-code
```javascript
function Agent(consul) {
  this.consul = consul;
  this.check = new Agent.Check(consul);
  this.service = new Agent.Service(consul);
}
```
- example usage
```shell
...
  if (defaults) this._defaults = defaults;
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);
...
```

#### <a name="apidoc.element.consul.Agent.Check"></a>[function <span class="apidocSignatureSpan">consul.Agent.</span>Check (consul)](#apidoc.element.consul.Agent.Check)
- description and source-code
```javascript
function AgentCheck(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

/**
 * Initialize a new 'Agent' client.
 */

function Agent(consul) {
  this.consul = consul;
  this.check = new Agent.Check(consul);
  this.service = new Agent.Service(consul);
}

Agent.Check = AgentCheck;
Agent.Service = AgentService;

/**
...
```

#### <a name="apidoc.element.consul.Agent.Service"></a>[function <span class="apidocSignatureSpan">consul.Agent.</span>Service (consul)](#apidoc.element.consul.Agent.Service)
- description and source-code
```javascript
function AgentService(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
/**
* Initialize a new 'Agent' client.
*/

function Agent(consul) {
 this.consul = consul;
 this.check = new Agent.Check(consul);
 this.service = new Agent.Service(consul);
}

Agent.Check = AgentCheck;
Agent.Service = AgentService;

/**
* Returns the checks the local agent is managing
...
```



# <a name="apidoc.module.consul.Agent.Check"></a>[module consul.Agent.Check](#apidoc.module.consul.Agent.Check)

#### <a name="apidoc.element.consul.Agent.Check.Check"></a>[function <span class="apidocSignatureSpan">consul.Agent.</span>Check (consul)](#apidoc.element.consul.Agent.Check.Check)
- description and source-code
```javascript
function AgentCheck(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

/**
 * Initialize a new 'Agent' client.
 */

function Agent(consul) {
  this.consul = consul;
  this.check = new Agent.Check(consul);
  this.service = new Agent.Service(consul);
}

Agent.Check = AgentCheck;
Agent.Service = AgentService;

/**
...
```



# <a name="apidoc.module.consul.Agent.Check.prototype"></a>[module consul.Agent.Check.prototype](#apidoc.module.consul.Agent.Check.prototype)

#### <a name="apidoc.element.consul.Agent.Check.prototype.deregister"></a>[function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>deregister (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.deregister)
- description and source-code
```javascript
deregister = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.check.deregister',
    path: '/agent/check/deregister/{id}',
    params: { id: opts.id },
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...

consul.agent.check.register(check, function(err) {
 if (err) throw err;
});
'''

<a name="agent-check-deregister"></a>
### consul.agent.check.deregister(options, callback)

Deregister a check.

Options

* id (String): check ID
...
```

#### <a name="apidoc.element.consul.Agent.Check.prototype.fail"></a>[function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>fail (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.fail)
- description and source-code
```javascript
fail = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.check.fail',
    path: '/agent/check/fail/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  if (opts.note) req.query.note = opts.note;

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.agent.check.warn('example', function(err) {
 if (err) throw err;
});
'''

<a name="agent-check-fail"></a>
### consul.agent.check.fail(options, callback)

Mark a test as critical.

Options

* id (String): check ID
* note (String, optional): human readable message
...
```

#### <a name="apidoc.element.consul.Agent.Check.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>list (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.check.list',
    path: '/agent/checks',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Agent.Check.prototype.pass"></a>[function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>pass (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.pass)
- description and source-code
```javascript
pass = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.check.pass',
    path: '/agent/check/pass/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  if (opts.note) req.query.note = opts.note;

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.agent.check.deregister('example', function(err) {
 if (err) throw err;
});
'''

<a name="agent-check-pass"></a>
### consul.agent.check.pass(options, callback)

Mark a test as passing.

Options

* id (String): check ID
* note (String, optional): human readable message
...
```

#### <a name="apidoc.element.consul.Agent.Check.prototype.register"></a>[function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>register (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.register)
- description and source-code
```javascript
register = function (opts, callback) {
  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.check.register',
    path: '/agent/check/register',
    type: 'json',
  };

  try {
    req.body = utils.createCheck(opts);
  } catch (err) {
    return callback(this.consul._err(errors.Validation(err.message), req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
   "ServiceID": "",
   "ServiceName": ""
 }
}
'''

<a name="agent-check-register"></a>
### consul.agent.check.register(options, callback)

Registers a new check.

Options

* name (String): check name
* id (String, optional): check ID
...
```

#### <a name="apidoc.element.consul.Agent.Check.prototype.warn"></a>[function <span class="apidocSignatureSpan">consul.Agent.Check.prototype.</span>warn (opts, callback)](#apidoc.element.consul.Agent.Check.prototype.warn)
- description and source-code
```javascript
warn = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.check.warn',
    path: '/agent/check/warn/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  if (opts.note) req.query.note = opts.note;

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.agent.check.pass('example', function(err) {
 if (err) throw err;
});
'''

<a name="agent-check-warn"></a>
### consul.agent.check.warn(options, callback)

Mark a test as warning.

Options

* id (String): check ID
* note (String, optional): human readable message
...
```



# <a name="apidoc.module.consul.Agent.Service"></a>[module consul.Agent.Service](#apidoc.module.consul.Agent.Service)

#### <a name="apidoc.element.consul.Agent.Service.Service"></a>[function <span class="apidocSignatureSpan">consul.Agent.</span>Service (consul)](#apidoc.element.consul.Agent.Service.Service)
- description and source-code
```javascript
function AgentService(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
/**
* Initialize a new 'Agent' client.
*/

function Agent(consul) {
 this.consul = consul;
 this.check = new Agent.Check(consul);
 this.service = new Agent.Service(consul);
}

Agent.Check = AgentCheck;
Agent.Service = AgentService;

/**
* Returns the checks the local agent is managing
...
```



# <a name="apidoc.module.consul.Agent.Service.prototype"></a>[module consul.Agent.Service.prototype](#apidoc.module.consul.Agent.Service.prototype)

#### <a name="apidoc.element.consul.Agent.Service.prototype.deregister"></a>[function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>deregister (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.deregister)
- description and source-code
```javascript
deregister = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.service.deregister',
    path: '/agent/service/deregister/{id}',
    params: { id: opts.id },
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...

consul.agent.check.register(check, function(err) {
 if (err) throw err;
});
'''

<a name="agent-check-deregister"></a>
### consul.agent.check.deregister(options, callback)

Deregister a check.

Options

* id (String): check ID
...
```

#### <a name="apidoc.element.consul.Agent.Service.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>list (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.service.list',
    path: '/agent/services',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Agent.Service.prototype.maintenance"></a>[function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>maintenance (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.maintenance)
- description and source-code
```javascript
maintenance = function (opts, callback) {
  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.service.maintenance',
    path: '/agent/service/maintenance/{id}',
    params: { id: opts.id },
    query: { enable: opts.enable },
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }
  if (typeof opts.enable !== 'boolean') {
    return callback(this.consul._err(errors.Validation('enable required'), req));
  }
  if (opts.reason) req.query.reason = opts.reason;

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
   "DelegateMax": 4,
   "DelegateCur": 4
 }
}
'''

<a name="agent-maintenance"></a>
### consul.agent.maintenance(options, callback)

Set node maintenance mode.

Options

* enable (Boolean): maintenance mode enabled
* reason (String, optional): human readable reason for maintenance
...
```

#### <a name="apidoc.element.consul.Agent.Service.prototype.register"></a>[function <span class="apidocSignatureSpan">consul.Agent.Service.prototype.</span>register (opts, callback)](#apidoc.element.consul.Agent.Service.prototype.register)
- description and source-code
```javascript
register = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { name: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.service.register',
    path: '/agent/service/register',
    type: 'json',
    body: {},
  };

  if (!opts.name) {
    return callback(this.consul._err(errors.Validation('name required'), req));
  }

  req.body.Name = opts.name;
  if (opts.id) req.body.ID = opts.id;
  if (opts.tags) req.body.Tags = opts.tags;
  if (opts.hasOwnProperty('address')) req.body.Address = opts.address;
  if (opts.hasOwnProperty('port')) req.body.Port = opts.port;

  try {
    if (Array.isArray(opts.checks)) {
      req.body.Checks = opts.checks.map(utils.createServiceCheck);
    } else if (opts.check) {
      req.body.Check = utils.createServiceCheck(opts.check);
    }
  } catch (err) {
    return callback(this.consul._err(errors.Validation(err.message), req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
   "ServiceID": "",
   "ServiceName": ""
 }
}
'''

<a name="agent-check-register"></a>
### consul.agent.check.register(options, callback)

Registers a new check.

Options

* name (String): check name
* id (String, optional): check ID
...
```



# <a name="apidoc.module.consul.Agent.prototype"></a>[module consul.Agent.prototype](#apidoc.module.consul.Agent.prototype)

#### <a name="apidoc.element.consul.Agent.prototype.checks"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>checks ()](#apidoc.element.consul.Agent.prototype.checks)
- description and source-code
```javascript
checks = function () {
  this.check.list.apply(this.check, arguments);
}
```
- example usage
```shell
...
   "ServiceID": "example",
   "ServiceName": "example"
 }
]
'''

<a name="health-checks"></a>
### consul.health.checks(options, callback)

Returns the checks of a service.

Options

* service (String): service name
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Agent.prototype.forceLeave"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>forceLeave (opts, callback)](#apidoc.element.consul.Agent.prototype.forceLeave)
- description and source-code
```javascript
forceLeave = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { node: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.forceLeave',
    path: '/agent/force-leave/{node}',
    params: { node: opts.node },
  };

  if (!opts.node) {
    return callback(this.consul._err(errors.Validation('node required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.agent.join('127.0.0.2', function(err) {
 if (err) throw err;
});
'''

<a name="agent-force-leave"></a>
### consul.agent.forceLeave(options, callback)

Force remove node.

Options

* node (String): node name to remove
...
```

#### <a name="apidoc.element.consul.Agent.prototype.join"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>join (opts, callback)](#apidoc.element.consul.Agent.prototype.join)
- description and source-code
```javascript
join = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { address: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.join',
    path: '/agent/join/{address}',
    params: { address: opts.address },
  };

  if (!opts.address) {
    return callback(this.consul._err(errors.Validation('address required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.agent.maintenance(true, function(err) {
 if (err) throw err;
});
'''

<a name="agent-join"></a>
### consul.agent.join(options, callback)

Trigger agent to join a node.

Options

* address (String): node IP address to join
* wan (Boolean, default false): attempt to join using the WAN pool
...
```

#### <a name="apidoc.element.consul.Agent.prototype.maintenance"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>maintenance (opts, callback)](#apidoc.element.consul.Agent.prototype.maintenance)
- description and source-code
```javascript
maintenance = function (opts, callback) {
  if (typeof opts === 'boolean') {
    opts = { enable: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.maintenance',
    path: '/agent/maintenance',
    query: { enable: opts.enable },
  };

  if (typeof opts.enable !== 'boolean') {
    return callback(this.consul._err(errors.Validation('enable required'), req));
  }
  if (opts.reason) req.query.reason = opts.reason;

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
   "DelegateMax": 4,
   "DelegateCur": 4
 }
}
'''

<a name="agent-maintenance"></a>
### consul.agent.maintenance(options, callback)

Set node maintenance mode.

Options

* enable (Boolean): maintenance mode enabled
* reason (String, optional): human readable reason for maintenance
...
```

#### <a name="apidoc.element.consul.Agent.prototype.members"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>members (opts, callback)](#apidoc.element.consul.Agent.prototype.members)
- description and source-code
```javascript
members = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.members',
    path: '/agent/members',
    query: {},
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
* [members](#agent-members)
* [self](#agent-self)
* [maintenance](#agent-maintenance)
* [join](#agent-join)
* [forceLeave](#agent-force-leave)

<a name="agent-members"></a>
### consul.agent.members([options], callback)

Returns the members as seen by the consul agent.

Options

* wan (Boolean, default: false): return WAN members instead of LAN members
...
```

#### <a name="apidoc.element.consul.Agent.prototype.self"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>self (opts, callback)](#apidoc.element.consul.Agent.prototype.self)
- description and source-code
```javascript
self = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'agent.self',
    path: '/agent/self',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
    "DelegateMax": 4,
    "DelegateCur": 4
  }
]
'''

<a name="agent-self"></a>
### consul.agent.self(callback)

Returns the agent node configuration.

Usage

''' javascript
consul.agent.self(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Agent.prototype.services"></a>[function <span class="apidocSignatureSpan">consul.Agent.prototype.</span>services ()](#apidoc.element.consul.Agent.prototype.services)
- description and source-code
```javascript
services = function () {
  this.service.list.apply(this.service, arguments);
}
```
- example usage
```shell
...
   "Node": "node1",
   "Address": "127.0.0.1"
 }
]
'''

<a name="catalog-node-services"></a>
### consul.catalog.node.services(options, callback)

Lists the services provided by a node.

Options

* node (String): node ID
...
```



# <a name="apidoc.module.consul.Catalog"></a>[module consul.Catalog](#apidoc.module.consul.Catalog)

#### <a name="apidoc.element.consul.Catalog.Catalog"></a>[function <span class="apidocSignatureSpan">consul.</span>Catalog (consul)](#apidoc.element.consul.Catalog.Catalog)
- description and source-code
```javascript
function Catalog(consul) {
  this.consul = consul;
  this.node = new Catalog.Node(consul);
  this.service = new Catalog.Service(consul);
}
```
- example usage
```shell
...
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);
...
```

#### <a name="apidoc.element.consul.Catalog.Node"></a>[function <span class="apidocSignatureSpan">consul.Catalog.</span>Node (consul)](#apidoc.element.consul.Catalog.Node)
- description and source-code
```javascript
function CatalogNode(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

/**
 * Initialize a new 'Catalog' client.
 */

function Catalog(consul) {
  this.consul = consul;
  this.node = new Catalog.Node(consul);
  this.service = new Catalog.Service(consul);
}

Catalog.Node = CatalogNode;
Catalog.Service = CatalogService;

/**
...
```

#### <a name="apidoc.element.consul.Catalog.Service"></a>[function <span class="apidocSignatureSpan">consul.Catalog.</span>Service (consul)](#apidoc.element.consul.Catalog.Service)
- description and source-code
```javascript
function CatalogService(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
/**
* Initialize a new 'Agent' client.
*/

function Agent(consul) {
 this.consul = consul;
 this.check = new Agent.Check(consul);
 this.service = new Agent.Service(consul);
}

Agent.Check = AgentCheck;
Agent.Service = AgentService;

/**
* Returns the checks the local agent is managing
...
```



# <a name="apidoc.module.consul.Catalog.Node"></a>[module consul.Catalog.Node](#apidoc.module.consul.Catalog.Node)

#### <a name="apidoc.element.consul.Catalog.Node.Node"></a>[function <span class="apidocSignatureSpan">consul.Catalog.</span>Node (consul)](#apidoc.element.consul.Catalog.Node.Node)
- description and source-code
```javascript
function CatalogNode(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

/**
 * Initialize a new 'Catalog' client.
 */

function Catalog(consul) {
  this.consul = consul;
  this.node = new Catalog.Node(consul);
  this.service = new Catalog.Service(consul);
}

Catalog.Node = CatalogNode;
Catalog.Service = CatalogService;

/**
...
```



# <a name="apidoc.module.consul.Catalog.Node.prototype"></a>[module consul.Catalog.Node.prototype](#apidoc.module.consul.Catalog.Node.prototype)

#### <a name="apidoc.element.consul.Catalog.Node.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Catalog.Node.prototype.</span>list (opts, callback)](#apidoc.element.consul.Catalog.Node.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  } else if (typeof opts === 'string') {
    opts = { dc: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'catalog.node.list',
    path: '/catalog/nodes',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Catalog.Node.prototype.services"></a>[function <span class="apidocSignatureSpan">consul.Catalog.Node.prototype.</span>services (opts, callback)](#apidoc.element.consul.Catalog.Node.prototype.services)
- description and source-code
```javascript
services = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { node: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'catalog.node.services',
    path: '/catalog/node/{node}',
    params: { node: opts.node },
  };

  if (!opts.node) {
    return callback(this.consul._err(errors.Validation('node required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
   "Node": "node1",
   "Address": "127.0.0.1"
 }
]
'''

<a name="catalog-node-services"></a>
### consul.catalog.node.services(options, callback)

Lists the services provided by a node.

Options

* node (String): node ID
...
```



# <a name="apidoc.module.consul.Catalog.Service"></a>[module consul.Catalog.Service](#apidoc.module.consul.Catalog.Service)

#### <a name="apidoc.element.consul.Catalog.Service.Service"></a>[function <span class="apidocSignatureSpan">consul.Catalog.</span>Service (consul)](#apidoc.element.consul.Catalog.Service.Service)
- description and source-code
```javascript
function CatalogService(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
/**
* Initialize a new 'Agent' client.
*/

function Agent(consul) {
 this.consul = consul;
 this.check = new Agent.Check(consul);
 this.service = new Agent.Service(consul);
}

Agent.Check = AgentCheck;
Agent.Service = AgentService;

/**
* Returns the checks the local agent is managing
...
```



# <a name="apidoc.module.consul.Catalog.Service.prototype"></a>[module consul.Catalog.Service.prototype](#apidoc.module.consul.Catalog.Service.prototype)

#### <a name="apidoc.element.consul.Catalog.Service.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Catalog.Service.prototype.</span>list (opts, callback)](#apidoc.element.consul.Catalog.Service.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  } else if (typeof opts === 'string') {
    opts = { dc: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'catalog.service.list',
    path: '/catalog/services',
    query: {},
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Catalog.Service.prototype.nodes"></a>[function <span class="apidocSignatureSpan">consul.Catalog.Service.prototype.</span>nodes (opts, callback)](#apidoc.element.consul.Catalog.Service.prototype.nodes)
- description and source-code
```javascript
nodes = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { service: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'catalog.service.nodes',
    path: '/catalog/service/{service}',
    params: { service: opts.service },
    query: {},
  };

  if (!opts.service) {
    return callback(this.consul._err(errors.Validation('service required'), req));
  }
  if (opts.tag) req.query.tag = opts.tag;

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
   "dev",
   "web"
 ]
}
'''

<a name="catalog-service-nodes"></a>
### consul.catalog.service.nodes(options, callback)

Lists the nodes in a given service.

Options

* service (String): service name
* dc (String, optional): datacenter (defaults to local for agent)
...
```



# <a name="apidoc.module.consul.Catalog.prototype"></a>[module consul.Catalog.prototype](#apidoc.module.consul.Catalog.prototype)

#### <a name="apidoc.element.consul.Catalog.prototype.datacenters"></a>[function <span class="apidocSignatureSpan">consul.Catalog.prototype.</span>datacenters (opts, callback)](#apidoc.element.consul.Catalog.prototype.datacenters)
- description and source-code
```javascript
datacenters = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'catalog.datacenters',
    path: '/catalog/datacenters',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
### consul.catalog

 * [node](#catalog-node)
 * [service](#catalog-service)
 * [datacenters](#catalog-datacenters)

<a name="catalog-datacenters"></a>
### consul.catalog.datacenters(callback)

Lists known datacenters.

Usage

''' javascript
consul.catalog.datacenters(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Catalog.prototype.nodes"></a>[function <span class="apidocSignatureSpan">consul.Catalog.prototype.</span>nodes ()](#apidoc.element.consul.Catalog.prototype.nodes)
- description and source-code
```javascript
nodes = function () {
  this.node.list.apply(this.node, arguments);
}
```
- example usage
```shell
...
   "dev",
   "web"
 ]
}
'''

<a name="catalog-service-nodes"></a>
### consul.catalog.service.nodes(options, callback)

Lists the nodes in a given service.

Options

* service (String): service name
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Catalog.prototype.services"></a>[function <span class="apidocSignatureSpan">consul.Catalog.prototype.</span>services ()](#apidoc.element.consul.Catalog.prototype.services)
- description and source-code
```javascript
services = function () {
  this.service.list.apply(this.service, arguments);
}
```
- example usage
```shell
...
   "Node": "node1",
   "Address": "127.0.0.1"
 }
]
'''

<a name="catalog-node-services"></a>
### consul.catalog.node.services(options, callback)

Lists the services provided by a node.

Options

* node (String): node ID
...
```



# <a name="apidoc.module.consul.Event"></a>[module consul.Event](#apidoc.module.consul.Event)

#### <a name="apidoc.element.consul.Event.Event"></a>[function <span class="apidocSignatureSpan">consul.</span>Event (consul)](#apidoc.element.consul.Event.Event)
- description and source-code
```javascript
function Event(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
...
```



# <a name="apidoc.module.consul.Event.prototype"></a>[module consul.Event.prototype](#apidoc.module.consul.Event.prototype)

#### <a name="apidoc.element.consul.Event.prototype.fire"></a>[function <span class="apidocSignatureSpan">consul.Event.prototype.</span>fire (opts, callback)](#apidoc.element.consul.Event.prototype.fire)
- description and source-code
```javascript
fire = function (opts, callback) {
  if (arguments.length === 3) {
    opts = {
      name: arguments[0],
      payload: arguments[1],
    };
    callback = arguments[2];
  } else if (typeof opts === 'string') {
    opts = { name: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'event.fire',
    path: '/event/fire/{name}',
    params: { name: opts.name },
    query: {},
  };

  if (!opts.name) {
    return callback(this.consul._err(errors.Validation('name required'), req));
  }

  var buffer;

  if (opts.hasOwnProperty('payload')) {
    buffer = Buffer.isBuffer(opts.payload);
    req.body = buffer ? opts.payload : new Buffer(opts.payload);
  }
  if (opts.node) req.query.node = opts.node;
  if (opts.service) req.query.service = opts.service;
  if (opts.tag) req.query.tag = opts.tag;

  utils.options(req, opts);

  this.consul._put(req, utils.body, function(err, data, res) {
    if (err) return callback(err, undefined, res);

    if (data.hasOwnProperty('Payload')) {
      data.Payload = utils.decode(data.Payload, { buffer: buffer });
    }

    callback(null, data, res);
  });
}
```
- example usage
```shell
...
<a name="event"></a>
### consul.event

* [fire](#event-fire)
* [list](#event-list)

<a name="event-fire"></a>
### consul.event.fire(options, callback)

Fires a new user event.

Options

* name (String): event name
* payload (String|Buffer): payload
...
```

#### <a name="apidoc.element.consul.Event.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Event.prototype.</span>list (opts, callback)](#apidoc.element.consul.Event.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { name: opts };
  } else if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'event.list',
    path: '/event/list',
    query: {},
  };

  if (opts.name) req.query.name = opts.name;

  utils.options(req, opts);

  this.consul._get(req, utils.body, function(err, data, res) {
    if (err) return callback(err, undefined, res);

    data.forEach(function(item) {
      if (!item.hasOwnProperty('Payload')) return;
      item.Payload = utils.decode(item.Payload, opts);
    });

    callback(null, data, res);
  });
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```



# <a name="apidoc.module.consul.Health"></a>[module consul.Health](#apidoc.module.consul.Health)

#### <a name="apidoc.element.consul.Health.Health"></a>[function <span class="apidocSignatureSpan">consul.</span>Health (consul)](#apidoc.element.consul.Health.Health)
- description and source-code
```javascript
function Health(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
...
```



# <a name="apidoc.module.consul.Health.prototype"></a>[module consul.Health.prototype](#apidoc.module.consul.Health.prototype)

#### <a name="apidoc.element.consul.Health.prototype.checks"></a>[function <span class="apidocSignatureSpan">consul.Health.prototype.</span>checks (opts, callback)](#apidoc.element.consul.Health.prototype.checks)
- description and source-code
```javascript
checks = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { service: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'health.checks',
    path: '/health/checks/{service}',
    params: { service: opts.service },
  };

  if (!opts.service) {
    return callback(this.consul._err(errors.Validation('service required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
   "ServiceID": "example",
   "ServiceName": "example"
 }
]
'''

<a name="health-checks"></a>
### consul.health.checks(options, callback)

Returns the checks of a service.

Options

* service (String): service name
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Health.prototype.node"></a>[function <span class="apidocSignatureSpan">consul.Health.prototype.</span>node (opts, callback)](#apidoc.element.consul.Health.prototype.node)
- description and source-code
```javascript
node = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { node: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'health.node',
    path: '/health/node/{node}',
    params: { node: opts.node },
  };

  if (!opts.node) {
    return callback(this.consul._err(errors.Validation('node required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...

* [node](#health-node)
* [checks](#health-checks)
* [service](#health-service)
* [state](#health-state)

<a name="health-node"></a>
### consul.health.node(options, callback)

Returns the health info of a node.

Options

* node (String): node
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Health.prototype.service"></a>[function <span class="apidocSignatureSpan">consul.Health.prototype.</span>service (opts, callback)](#apidoc.element.consul.Health.prototype.service)
- description and source-code
```javascript
service = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { service: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'health.service',
    path: '/health/service/{service}',
    params: { service: opts.service },
    query: {},
  };

  if (!opts.service) {
    return callback(this.consul._err(errors.Validation('service required'), req));
  }

  if (opts.tag) req.query.tag = opts.tag;
  if (opts.passing) req.query.passing = 'true';

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
   "ServiceID": "example",
   "ServiceName": "example"
 }
]
'''

<a name="health-service"></a>
### consul.health.service(options, callback)

Returns the nodes and health info of a service.

Options

* service (String): service name
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Health.prototype.state"></a>[function <span class="apidocSignatureSpan">consul.Health.prototype.</span>state (opts, callback)](#apidoc.element.consul.Health.prototype.state)
- description and source-code
```javascript
state = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { state: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'health.state',
    path: '/health/state/{state}',
    params: { state: opts.state },
  };

  if (!opts.state) {
    return callback(this.consul._err(errors.Validation('state required'), req));
  }

  if (opts.state !== 'any' && constants.CHECK_STATE.indexOf(opts.state) < 0) {
    return callback(this.consul._err(errors.Validation('state invalid: ' + opts.state), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
     }
   ]
 }
]
'''

<a name="health-state"></a>
### consul.health.state(options, callback)

Returns the checks in a given state.

Options

* state (String, enum: any, passing, warning, critical): state
* dc (String, optional): datacenter (defaults to local for agent)
...
```



# <a name="apidoc.module.consul.Kv"></a>[module consul.Kv](#apidoc.module.consul.Kv)

#### <a name="apidoc.element.consul.Kv.Kv"></a>[function <span class="apidocSignatureSpan">consul.</span>Kv (consul)](#apidoc.element.consul.Kv.Kv)
- description and source-code
```javascript
function Kv(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
...
```



# <a name="apidoc.module.consul.Kv.prototype"></a>[module consul.Kv.prototype](#apidoc.module.consul.Kv.prototype)

#### <a name="apidoc.element.consul.Kv.prototype.del"></a>[function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>del (opts, callback)](#apidoc.element.consul.Kv.prototype.del)
- description and source-code
```javascript
del = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { key: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'kv.del',
    path: '/kv/{key}',
    params: { key: (opts.key || '') },
    query: {},
  };

  if (opts.recurse) req.query.recurse = 'true';

  if (opts.hasOwnProperty('cas')) req.query.cas = opts.cas;

  utils.options(req, opts);

  this.consul._delete(req, utils.empty, callback);
}
```
- example usage
```shell
...
Result

''' json
true
'''

<a name="kv-del"></a>
### consul.kv.del(options, callback)

Delete key/value (kv) pair(s).

Options

* key (String): key
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Kv.prototype.delete"></a>[function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>delete (opts, callback)](#apidoc.element.consul.Kv.prototype.delete)
- description and source-code
```javascript
delete = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { key: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'kv.del',
    path: '/kv/{key}',
    params: { key: (opts.key || '') },
    query: {},
  };

  if (opts.recurse) req.query.recurse = 'true';

  if (opts.hasOwnProperty('cas')) req.query.cas = opts.cas;

  utils.options(req, opts);

  this.consul._delete(req, utils.empty, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Kv.prototype.get"></a>[function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>get (opts, callback)](#apidoc.element.consul.Kv.prototype.get)
- description and source-code
```javascript
get = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { key: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'kv.get',
    path: '/kv/{key}',
    params: { key: (opts.key || '') },
    query: {},
  };

  if (opts.recurse) req.query.recurse = 'true';
  if (opts.raw) {
    req.query.raw = 'true';
    req.buffer = true;
  }

  utils.options(req, opts);

  this.consul._get(req, function(err, res) {
    if (res && res.statusCode === 404) return callback(undefined, undefined, res);
    if (err) return callback(err, undefined, res);
    if (opts.raw) return callback(null, res.body, res);

    if (res.body && Array.isArray(res.body) && res.body.length) {
      res.body.forEach(function(item) {
        if (!item.hasOwnProperty('Value')) return;
        item.Value = utils.decode(item.Value, opts);
      });
    } else {
      return callback(undefined, undefined, res);
    }

    if (!opts.recurse) return callback(null, res.body[0], res);

    callback(null, res.body, res);
  });
}
```
- example usage
```shell
...
''' javascript
consul.acl.destroy('b1f4c10e-b61b-e1de-de95-218c9fefdd3e', function(err) {
 if (err) throw err;
});
'''

<a name="acl-get"></a>
### consul.acl.get(options, callback)

Queries the policy of a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Kv.prototype.keys"></a>[function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>keys (opts, callback)](#apidoc.element.consul.Kv.prototype.keys)
- description and source-code
```javascript
keys = function (opts, callback) {
  switch (typeof opts) {
    case 'string':
      opts = { key: opts };
      break;
    case 'function':
      callback = opts;
      opts = {};
      break;
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'kv.keys',
    path: '/kv/{key}',
    params: { key: (opts.key || '') },
    query: { keys: true },
  };

  if (opts.separator) req.query.separator = opts.separator;

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
 "Key": "hello",
 "Flags": 0,
 "Value": "world"
}
'''

<a name="kv-keys"></a>
### consul.kv.keys(options, callback)

Return keys for a given prefix.

Options

* key (String): path prefix
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Kv.prototype.set"></a>[function <span class="apidocSignatureSpan">consul.Kv.prototype.</span>set (opts, callback)](#apidoc.element.consul.Kv.prototype.set)
- description and source-code
```javascript
set = function (opts, callback) {
  switch (arguments.length) {
    case 4:
      // set(key, value, opts, callback)
      opts = arguments[2];
      opts.key = arguments[0];
      opts.value = arguments[1];
      callback = arguments[3];
      break;
    case 3:
      // set(key, value, callback)
      opts = {
        key: arguments[0],
        value: arguments[1],
      };
      callback = arguments[2];
      break;
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'kv.set',
    path: '/kv/{key}',
    params: { key: opts.key },
    query: {},
    type: 'text',
    body: opts.value || '',
  };

  if (!opts.key) {
    return callback(this.consul._err(errors.Validation('key required'), req));
  }
  if (!opts.hasOwnProperty('value')) {
    return callback(this.consul._err(errors.Validation('value required'), req));
  }

  if (opts.hasOwnProperty('cas')) req.query.cas = opts.cas;
  if (opts.hasOwnProperty('flags')) req.query.flags = opts.flags;
  if (opts.hasOwnProperty('acquire')) req.query.acquire = opts.acquire;
  if (opts.hasOwnProperty('release')) req.query.release = opts.release;

  utils.options(req, opts);

  this.consul._put(req, utils.body, callback);
}
```
- example usage
```shell
...
[
 "a/b",
 "a/c"
]
'''

<a name="kv-set"></a>
### consul.kv.set(options, callback)

Set key/value (kv) pair.

Options

* key (String): key
* value (String|Buffer): value
...
```



# <a name="apidoc.module.consul.Lock"></a>[module consul.Lock](#apidoc.module.consul.Lock)

#### <a name="apidoc.element.consul.Lock.Lock"></a>[function <span class="apidocSignatureSpan">consul.</span>Lock (consul, opts)](#apidoc.element.consul.Lock.Lock)
- description and source-code
```javascript
function Lock(consul, opts) {
  events.EventEmitter.call(this);

  opts = utils.normalizeKeys(opts);

  this.consul = consul;
  this._opts = opts;

  if (opts.session) {
    switch (typeof opts.session) {
      case 'string':
        opts.session = { id: opts.session };
        break;
      case 'object':
        opts.session = utils.normalizeKeys(opts.session);
        break;
      default:
        throw errors.Validation('session must be an object or string');
    }
  } else {
    opts.session = {};
  }

  if (!opts.key) {
    throw errors.Validation('key required');
  } else if (typeof opts.key !== 'string') {
    throw errors.Validation('key must be a string');
  }
}
```
- example usage
```shell
...
/**
 * Lock helper.
 */

Consul.meta.lock = { type: 'eventemitter' };

Consul.prototype.lock = function(opts) {
  return new Consul.Lock(this, opts);
};

/**
 * Watch helper.
 */

Consul.meta.watch = { type: 'eventemitter' };
...
```

#### <a name="apidoc.element.consul.Lock.super_"></a>[function <span class="apidocSignatureSpan">consul.Lock.</span>super_ ()](#apidoc.element.consul.Lock.super_)
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



# <a name="apidoc.module.consul.Lock.prototype"></a>[module consul.Lock.prototype](#apidoc.module.consul.Lock.prototype)

#### <a name="apidoc.element.consul.Lock.prototype._acquire"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_acquire (ctx)](#apidoc.element.consul.Lock.prototype._acquire)
- description and source-code
```javascript
_acquire = function (ctx) {
  var self = this;

  var opts = utils.defaults({
    key: ctx.key,
    acquire: ctx.session.id,
    ctx: ctx,
    value: ctx.value,
    flags: LOCK_FLAG_VALUE,
  }, self.consul._defaults);

  self.consul.kv.set(opts, function(err, data, res) {
    if (err) return self._end(ctx, err, res);

    if (data !== true) {
      ctx.state = 'wait';

      return utils.setTimeoutContext(function() { self._run(ctx); }, ctx,
        ctx.lockRetryTime);
    }

    ctx.held = true;
    self.emit('acquire');

    ctx.state = 'monitor';

    self._run(ctx);
  });
}
```
- example usage
```shell
...

  switch (ctx.state) {
    case 'session':
      return this._session(ctx);
    case 'wait':
      return this._wait(ctx);
    case 'acquire':
      return this._acquire(ctx);
    case 'monitor':
      return this._monitor(ctx);
    default:
      throw new Error('invalid state: ' + ctx.state);
  }
};
...
```

#### <a name="apidoc.element.consul.Lock.prototype._end"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_end (ctx, err, res)](#apidoc.element.consul.Lock.prototype._end)
- description and source-code
```javascript
_end = function (ctx, err, res) {
  var self = this;

  if (ctx.end) return;
  ctx.end = true;

  delete self._ctx;

  if (err) self._err(err, res);

  if (ctx.monitor) {
    ctx.monitor.removeAllListeners();
    ctx.monitor.end();

    delete ctx.monitor;
  }

  if (ctx.renewSession) {
    clearInterval(ctx.renewSession);

    var opts = utils.defaults({
      id: ctx.session.id,
      timeout: 1000,
    }, self.consul._defaults);

    self.consul.session.destroy(opts, function() {
      // ignore errors
    });

    delete ctx.renewSession;
  }

  // abort any pending requests
  ctx.emit('cancel');

  if (ctx.held) {
    ctx.held = false;
    self.emit('release');
  }

  self.emit('end');
}
```
- example usage
```shell
...
ttl: ctx.session.ttl || DEFAULT_LOCK_SESSION_TTL,
ctx: ctx,
    }, ctx.session, self.consul._defaults);

    self.consul.session.create(opts, function(err, data, res) {
if (err) {
  err.message = 'session create: ' + err.message;
  return self._end(ctx, err, res);
}

ctx.session = {
  id: data.ID,
  ttl: opts.ttl,
};
...
```

#### <a name="apidoc.element.consul.Lock.prototype._err"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_err (err, res)](#apidoc.element.consul.Lock.prototype._err)
- description and source-code
```javascript
_err = function (err, res) {
  var self = this;

  self.emit('error', err, res);
}
```
- example usage
```shell
...
  path: '/acl/update',
  query: {},
  type: 'json',
  body: {},
};

if (!opts.id) {
  return callback(this.consul._err(errors.Validation('id required'), req));
}

req.body.ID = opts.id;

if (opts.name) req.body.Name = opts.name;
if (opts.type) req.body.Type = opts.type;
if (opts.rules) req.body.Rules = opts.rules;
...
```

#### <a name="apidoc.element.consul.Lock.prototype._monitor"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_monitor (ctx)](#apidoc.element.consul.Lock.prototype._monitor)
- description and source-code
```javascript
_monitor = function (ctx) {
  var self = this;

  var monitor = ctx.monitor = self.consul.watch({
    method: self.consul.kv.get,
    options: utils.defaults({
      key: ctx.key,
      wait: ctx.lockWaitTime,
      timeout: ctx.lockWaitTimeout,
      index: ctx.index,
    }, self.consul._defaults),
  });

  var ttl = ctx.session.ttl && utils.parseDuration(ctx.session.ttl);

  // monitor updates
  if (ttl) {
    utils.setIntervalContext(function() {
      var time = monitor.updateTime();

      if (time && new Date() - time > ttl + 1000) {
        monitor.end();
      }
    }, ctx, Math.min(1000, ttl));
  }

  monitor.on('change', function(data) {
    if (data) {
      if (data.Session !== ctx.session.id) {
        return monitor.end();
      }
    }
  });

  monitor.on('error', function() {
    // ignore errors
  });

  monitor.on('end', function() {
    self._end(ctx);
  });
}
```
- example usage
```shell
...
   case 'session':
     return this._session(ctx);
   case 'wait':
     return this._wait(ctx);
   case 'acquire':
     return this._acquire(ctx);
   case 'monitor':
     return this._monitor(ctx);
   default:
     throw new Error('invalid state: ' + ctx.state);
 }
};

/**
* Create lock session
...
```

#### <a name="apidoc.element.consul.Lock.prototype._release"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_release (ctx)](#apidoc.element.consul.Lock.prototype._release)
- description and source-code
```javascript
_release = function (ctx) {
  var self = this;

  if (ctx.held) {
    var opts = utils.defaults({
      key: ctx.key,
      release: ctx.session.id,
      ctx: ctx,
      value: ctx.value,
      flags: LOCK_FLAG_VALUE,
    }, self.consul._defaults);

    self.consul.kv.set(opts, function(err, data) {
      if (err) return self._end(ctx, err);

      if (data !== true) {
        err = new Error('failed to release lock');
        return self._end(ctx, err);
      }

      self._end(ctx);
    });

    return;
  }

  process.nextTick(function() {
    self._end(ctx);
  });
}
```
- example usage
```shell
...
 var ctx = self._ctx;

 if (!self._ctx) throw errors.Validation('no lock in use');

 delete self._ctx;

 process.nextTick(function() {
   self._release(ctx);
 });
};

/**
* Error helper
*/
...
```

#### <a name="apidoc.element.consul.Lock.prototype._run"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_run (ctx)](#apidoc.element.consul.Lock.prototype._run)
- description and source-code
```javascript
_run = function (ctx) {
  if (ctx.end) return;

  switch (ctx.state) {
    case 'session':
      return this._session(ctx);
    case 'wait':
      return this._wait(ctx);
    case 'acquire':
      return this._acquire(ctx);
    case 'monitor':
      return this._monitor(ctx);
    default:
      throw new Error('invalid state: ' + ctx.state);
  }
}
```
- example usage
```shell
...
 ctx.lockWaitTime = self._opts.lockwaittime || DEFAULT_LOCK_WAIT_TIME;
 ctx.lockWaitTimeout = utils.parseDuration(ctx.lockWaitTime) + 1000;
 ctx.lockRetryTime = utils.parseDuration(self._opts.lockretrytime || DEFAULT_LOCK_RETRY_TIME);
 ctx.state = 'session';
 ctx.value = self._opts.value || null;

 process.nextTick(function() {
   self._run(ctx);
 });
};

/**
* Release lock
*/
...
```

#### <a name="apidoc.element.consul.Lock.prototype._session"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_session (ctx)](#apidoc.element.consul.Lock.prototype._session)
- description and source-code
```javascript
_session = function (ctx) {
  var self = this;

  if (!ctx.session.id) {
    var opts = utils.defaults({
      name: ctx.session.name || DEFAULT_LOCK_SESSION_NAME,
      ttl: ctx.session.ttl || DEFAULT_LOCK_SESSION_TTL,
      ctx: ctx,
    }, ctx.session, self.consul._defaults);

    self.consul.session.create(opts, function(err, data, res) {
      if (err) {
        err.message = 'session create: ' + err.message;
        return self._end(ctx, err, res);
      }

      ctx.session = {
        id: data.ID,
        ttl: opts.ttl,
      };

      ctx.state = 'wait';

      var renewTimeout = utils.parseDuration(ctx.session.ttl) / 2;

      // renew session
      ctx.renewSession = setInterval(function() {
        var opts = utils.defaults({
          id: ctx.session.id,
          timeout: renewTimeout,
          ctx: ctx,
        }, self.consul._defaults);

        self.consul.session.renew(opts, function(err, data, res) {
          if (err) self._end(ctx, err, res);
        });
      }, renewTimeout);

      return self._run(ctx);
    });

    return;
  }

  ctx.state = 'wait';

  process.nextTick(function() {
    self._run(ctx);
  });
}
```
- example usage
```shell
...
 */

Lock.prototype._run = function(ctx) {
if (ctx.end) return;

switch (ctx.state) {
  case 'session':
    return this._session(ctx);
  case 'wait':
    return this._wait(ctx);
  case 'acquire':
    return this._acquire(ctx);
  case 'monitor':
    return this._monitor(ctx);
  default:
...
```

#### <a name="apidoc.element.consul.Lock.prototype._wait"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>_wait (ctx)](#apidoc.element.consul.Lock.prototype._wait)
- description and source-code
```javascript
_wait = function (ctx) {
  var self = this;

  var retry = function() {
    utils.setTimeoutContext(function() {
      self._run(ctx);
    }, ctx, ctx.lockRetryTime);
  };

  var opts = utils.defaults({
    key: ctx.key,
    wait: ctx.lockWaitTime,
    timeout: ctx.lockWaitTimeout,
    ctx: ctx,
    index: ctx.index,
  }, self.consul._defaults);

  self.consul.kv.get(opts, function(err, data, res) {
    if (err) return self._end(ctx, err, res);

    if (data) {
      // we try to use the same magic number as consul/api in an attempt to be
      // compatible
      if (data.Flags !== +LOCK_FLAG_VALUE) {
        err = errors.Validation('consul: lock: existing key does not match lock use');
        return self._end(ctx, err, res);
      }

      var newIndex = res.headers['x-consul-index'];
      if (utils.hasIndexChanged(newIndex, ctx.index)) ctx.index = newIndex;

      if (data.Session !== ctx.Session) {
        self.emit('retry', { leader: data.Session });
        return retry();
      }
    } else if (res.statusCode !== 404) {
      return self._end(ctx, new Error('consul: lock: error getting key'), res);
    }

    ctx.state = 'acquire';

    self._run(ctx);
  });
}
```
- example usage
```shell
...
Lock.prototype._run = function(ctx) {
if (ctx.end) return;

switch (ctx.state) {
  case 'session':
    return this._session(ctx);
  case 'wait':
    return this._wait(ctx);
  case 'acquire':
    return this._acquire(ctx);
  case 'monitor':
    return this._monitor(ctx);
  default:
    throw new Error('invalid state: ' + ctx.state);
}
...
```

#### <a name="apidoc.element.consul.Lock.prototype.acquire"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>acquire ()](#apidoc.element.consul.Lock.prototype.acquire)
- description and source-code
```javascript
acquire = function () {
  var self = this;

  if (self._ctx) throw new errors.Validation('lock in use');

  var ctx = self._ctx = new events.EventEmitter();

  ctx.key = self._opts.key;
  ctx.session = utils.clone(self._opts.session);
  ctx.index = '0';
  ctx.end = false;
  ctx.lockWaitTime = self._opts.lockwaittime || DEFAULT_LOCK_WAIT_TIME;
  ctx.lockWaitTimeout = utils.parseDuration(ctx.lockWaitTime) + 1000;
  ctx.lockRetryTime = utils.parseDuration(self._opts.lockretrytime || DEFAULT_LOCK_RETRY_TIME);
  ctx.state = 'session';
  ctx.value = self._opts.value || null;

  process.nextTick(function() {
    self._run(ctx);
  });
}
```
- example usage
```shell
...
  console.log('lock error:', err);
});

lock.on('end', function(err) {
  console.log('lock released or there was a permanent failure');
});

lock.acquire();
'''

Result

'''
lock acquired
lock released
...
```

#### <a name="apidoc.element.consul.Lock.prototype.release"></a>[function <span class="apidocSignatureSpan">consul.Lock.prototype.</span>release ()](#apidoc.element.consul.Lock.prototype.release)
- description and source-code
```javascript
release = function () {
  var self = this;

  var ctx = self._ctx;

  if (!self._ctx) throw errors.Validation('no lock in use');

  delete self._ctx;

  process.nextTick(function() {
    self._release(ctx);
  });
}
```
- example usage
```shell
...

''' javascript
var lock = consul.lock({ key: 'test' });

lock.on('acquire', function() {
  console.log('lock acquired');

  lock.release();
});

lock.on('release', function() {
  console.log('lock released');
});

lock.on('error', function() {
...
```



# <a name="apidoc.module.consul.Query"></a>[module consul.Query](#apidoc.module.consul.Query)

#### <a name="apidoc.element.consul.Query.Query"></a>[function <span class="apidocSignatureSpan">consul.</span>Query (consul)](#apidoc.element.consul.Query.Query)
- description and source-code
```javascript
function Query(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
...
```



# <a name="apidoc.module.consul.Query.prototype"></a>[module consul.Query.prototype](#apidoc.module.consul.Query.prototype)

#### <a name="apidoc.element.consul.Query.prototype._params"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>_params (req, opts)](#apidoc.element.consul.Query.prototype._params)
- description and source-code
```javascript
_params = function (req, opts) {
  var body = req.body || {};

  if (opts.name) body.Name = opts.name;
  if (opts.session) body.Session = opts.session;
  if (opts.token) {
    body.Token = opts.token;
    delete opts.token;
  }
  if (opts.near) body.Near = opts.near;
  if (opts.template) {
    var template = utils.normalizeKeys(opts.template);
    if (template.type || template.regexp) {
      body.Template = {};
      if (template.type) body.Template.Type = template.type;
      if (template.regexp) body.Template.Regexp = template.regexp;
    }
  }
  if (opts.service) {
    var service = utils.normalizeKeys(opts.service);
    body.Service = {};
    if (service.service) body.Service.Service = service.service;
    if (service.failover) {
      var failover = utils.normalizeKeys(service.failover);
      if (typeof failover.nearestn === 'number' || failover.datacenters) {
        body.Service.Failover = {};
        if (typeof failover.nearestn === 'number') {
          body.Service.Failover.NearestN = failover.nearestn;
        }
        if (failover.datacenters) {
          body.Service.Failover.Datacenters = failover.datacenters;
        }
      }
    }
    if (typeof service.onlypassing === 'boolean') {
      body.Service.OnlyPassing = service.onlypassing;
    }
    if (service.tags) body.Service.Tags = service.tags;
  }
  if (opts.dns) {
    var dns = utils.normalizeKeys(opts.dns);
    if (dns.ttl) body.DNS = { TTL: dns.ttl };
  }

  req.body = body;
}
```
- example usage
```shell
...
  name: 'query.create',
  path: '/query',
  query: {},
  type: 'json',
};

try {
  this._params(req, opts);
  if (!req.body.Service || !req.body.Service.Service) {
    throw errors.Validation('service required');
  }
} catch (err) {
  return callback(this.consul._err(err, req));
}
...
```

#### <a name="apidoc.element.consul.Query.prototype.create"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>create (opts, callback)](#apidoc.element.consul.Query.prototype.create)
- description and source-code
```javascript
create = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { service: { service: opts } };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.create',
    path: '/query',
    query: {},
    type: 'json',
  };

  try {
    this._params(req, opts);
    if (!req.body.Service || !req.body.Service.Service) {
      throw errors.Validation('service required');
    }
  } catch (err) {
    return callback(this.consul._err(err, req));
  }

  utils.options(req, opts);

  this.consul._post(req, utils.body, callback);
}
```
- example usage
```shell
...
* [update](#acl-update)
* [destroy](#acl-destroy)
* [get](#acl-get)
* [clone](#acl-clone)
* [list](#acl-list)

<a name="acl-create"></a>
### consul.acl.create([options], callback)

Creates a new token with policy.

Options

* name (String, optional): human readable name for the token
* type (String, enum: client, management; default: client): type of token
...
```

#### <a name="apidoc.element.consul.Query.prototype.destroy"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>destroy (opts, callback)](#apidoc.element.consul.Query.prototype.destroy)
- description and source-code
```javascript
destroy = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { query: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.destroy',
    path: '/query/{query}',
    params: { query: opts.query },
    query: {},
  };

  if (!opts.query) {
    return callback(this.consul._err(errors.Validation('query required'), req));
  }

  utils.options(req, opts);

  this.consul._delete(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.acl.update({ id: '63e1d82e-f718-eb92-3b7d-61f0c71d45b4', name: 'test' }, function(err) {
 if (err) throw err;
});
'''

<a name="acl-destroy"></a>
### consul.acl.destroy(options, callback)

Destroys a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Query.prototype.execute"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>execute (opts, callback)](#apidoc.element.consul.Query.prototype.execute)
- description and source-code
```javascript
execute = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { query: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.execute',
    path: '/query/{query}/execute',
    params: { query: opts.query },
    query: {},
  };

  if (!opts.query) {
    return callback(this.consul._err(errors.Validation('query required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' javascript
consul.query.destroy('422b14b9-874b-4520-bd2e-e149a42b0066', function(err) {
 if (err) throw err;
});
'''

<a name="query-execute"></a>
### consul.query.execute(options, callback)

Execute prepared query.

Options

* query (String, required): ID of the query
...
```

#### <a name="apidoc.element.consul.Query.prototype.explain"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>explain (opts, callback)](#apidoc.element.consul.Query.prototype.explain)
- description and source-code
```javascript
explain = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { query: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.explain',
    path: '/query/{query}/explain',
    params: { query: opts.query },
    query: {},
  };

  if (!opts.query) {
    return callback(this.consul._err(errors.Validation('query required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.bodyItem, callback);
}
```
- example usage
```shell
...
     "Failovers": 2
   }
 ]
}
'''

<a name="query-explain"></a>
### consul.query.explain(options, callback)

Explain prepared query.

Options

* query (String, required): ID of the query
...
```

#### <a name="apidoc.element.consul.Query.prototype.get"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>get (opts, callback)](#apidoc.element.consul.Query.prototype.get)
- description and source-code
```javascript
get = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { query: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.get',
    path: '/query/{query}',
    params: { query: opts.query },
    query: {},
  };

  if (!opts.query) {
    return callback(this.consul._err(errors.Validation('query required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.bodyItem, callback);
}
```
- example usage
```shell
...
''' javascript
consul.acl.destroy('b1f4c10e-b61b-e1de-de95-218c9fefdd3e', function(err) {
 if (err) throw err;
});
'''

<a name="acl-get"></a>
### consul.acl.get(options, callback)

Queries the policy of a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Query.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>list (opts, callback)](#apidoc.element.consul.Query.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.list',
    path: '/query',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Query.prototype.update"></a>[function <span class="apidocSignatureSpan">consul.Query.prototype.</span>update (opts, callback)](#apidoc.element.consul.Query.prototype.update)
- description and source-code
```javascript
update = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'query.update',
    path: '/query/{query}',
    params: { query: opts.query },
    query: {},
    type: 'json',
  };

  try {
    if (!opts.query) throw errors.Validation('query required');
    this._params(req, opts);
    if (!req.body.Service || !req.body.Service.Service) {
      throw errors.Validation('service required');
    }
  } catch (err) {
    return callback(this.consul._err(err, req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' json
{
 "ID": "b1f4c10e-b61b-e1de-de95-218c9fefdd3e"
}
'''

<a name="acl-update"></a>
### consul.acl.update(options, callback)

Update the policy of a token.

Options

* id (String): token ID
* name (String, optional): human readable name for the token
...
```



# <a name="apidoc.module.consul.Session"></a>[module consul.Session](#apidoc.module.consul.Session)

#### <a name="apidoc.element.consul.Session.Session"></a>[function <span class="apidocSignatureSpan">consul.</span>Session (consul)](#apidoc.element.consul.Session.Session)
- description and source-code
```javascript
function Session(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
    } else {
...
```



# <a name="apidoc.module.consul.Session.prototype"></a>[module consul.Session.prototype](#apidoc.module.consul.Session.prototype)

#### <a name="apidoc.element.consul.Session.prototype.create"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>create (opts, callback)](#apidoc.element.consul.Session.prototype.create)
- description and source-code
```javascript
create = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.create',
    path: '/session/create',
    query: {},
    type: 'json',
    body: {},
  };

  if (opts.lockdelay) req.body.LockDelay = opts.lockdelay;
  if (opts.name) req.body.Name = opts.name;
  if (opts.node) req.body.Node = opts.node;
  if (opts.checks) req.body.Checks = opts.checks;
  if (opts.behavior) req.body.Behavior = opts.behavior;
  if (opts.ttl) req.body.TTL = opts.ttl;

  utils.options(req, opts);

  this.consul._put(req, utils.body, callback);
}
```
- example usage
```shell
...
* [update](#acl-update)
* [destroy](#acl-destroy)
* [get](#acl-get)
* [clone](#acl-clone)
* [list](#acl-list)

<a name="acl-create"></a>
### consul.acl.create([options], callback)

Creates a new token with policy.

Options

* name (String, optional): human readable name for the token
* type (String, enum: client, management; default: client): type of token
...
```

#### <a name="apidoc.element.consul.Session.prototype.destroy"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>destroy (opts, callback)](#apidoc.element.consul.Session.prototype.destroy)
- description and source-code
```javascript
destroy = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.destroy',
    path: '/session/destroy/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.empty, callback);
}
```
- example usage
```shell
...
''' javascript
consul.acl.update({ id: '63e1d82e-f718-eb92-3b7d-61f0c71d45b4', name: 'test' }, function(err) {
 if (err) throw err;
});
'''

<a name="acl-destroy"></a>
### consul.acl.destroy(options, callback)

Destroys a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Session.prototype.get"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>get (opts, callback)](#apidoc.element.consul.Session.prototype.get)
- description and source-code
```javascript
get = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.info',
    path: '/session/info/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.bodyItem, callback);
}
```
- example usage
```shell
...
''' javascript
consul.acl.destroy('b1f4c10e-b61b-e1de-de95-218c9fefdd3e', function(err) {
 if (err) throw err;
});
'''

<a name="acl-get"></a>
### consul.acl.get(options, callback)

Queries the policy of a given token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.Session.prototype.info"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>info (opts, callback)](#apidoc.element.consul.Session.prototype.info)
- description and source-code
```javascript
info = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.info',
    path: '/session/info/{id}',
    params: { id: opts.id },
    query: {},
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.bodyItem, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Session.prototype.list"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>list (opts, callback)](#apidoc.element.consul.Session.prototype.list)
- description and source-code
```javascript
list = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.list',
    path: '/session/list',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
''' json
{
  "ID": "9fb8b20b-2636-adbb-9b99-d879df3305ec"
}
'''

<a name="acl-list"></a>
### consul.acl.list([options], callback)

Lists all the active tokens.

Usage

''' javascript
consul.acl.list(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Session.prototype.node"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>node (opts, callback)](#apidoc.element.consul.Session.prototype.node)
- description and source-code
```javascript
node = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { node: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.node',
    path: '/session/node/{node}',
    params: { node: opts.node },
  };

  if (!opts.node) {
    return callback(this.consul._err(errors.Validation('node required'), req));
  }

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...

* [node](#health-node)
* [checks](#health-checks)
* [service](#health-service)
* [state](#health-state)

<a name="health-node"></a>
### consul.health.node(options, callback)

Returns the health info of a node.

Options

* node (String): node
* dc (String, optional): datacenter (defaults to local for agent)
...
```

#### <a name="apidoc.element.consul.Session.prototype.renew"></a>[function <span class="apidocSignatureSpan">consul.Session.prototype.</span>renew (opts, callback)](#apidoc.element.consul.Session.prototype.renew)
- description and source-code
```javascript
renew = function (opts, callback) {
  if (typeof opts === 'string') {
    opts = { id: opts };
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'session.renew',
    path: '/session/renew/{id}',
    params: { id: opts.id },
  };

  if (!opts.id) {
    return callback(this.consul._err(errors.Validation('id required'), req));
  }

  utils.options(req, opts);

  this.consul._put(req, utils.body, callback);
}
```
- example usage
```shell
...
   ],
   "LockDelay": 15000000000
 }
]
'''

<a name="session-renew"></a>
### consul.session.renew(options, callback)

Renew a given session.

Options

* id (String): session ID
* dc (String, optional): datacenter (defaults to local for agent)
...
```



# <a name="apidoc.module.consul.Status"></a>[module consul.Status](#apidoc.module.consul.Status)

#### <a name="apidoc.element.consul.Status.Status"></a>[function <span class="apidocSignatureSpan">consul.</span>Status (consul)](#apidoc.element.consul.Status.Status)
- description and source-code
```javascript
function Status(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
    } else {
      papi.tools.promisify(this);
...
```



# <a name="apidoc.module.consul.Status.prototype"></a>[module consul.Status.prototype](#apidoc.module.consul.Status.prototype)

#### <a name="apidoc.element.consul.Status.prototype.leader"></a>[function <span class="apidocSignatureSpan">consul.Status.prototype.</span>leader (opts, callback)](#apidoc.element.consul.Status.prototype.leader)
- description and source-code
```javascript
leader = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'status.leader',
    path: '/status/leader',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
<a name="status"></a>
### consul.status

 * [leader](#status-leader)
 * [peers](#status-peers)

<a name="status-leader"></a>
### consul.status.leader(callback)

Returns the current Raft leader.

Usage

''' javascript
consul.status.leader(function(err, result) {
...
```

#### <a name="apidoc.element.consul.Status.prototype.peers"></a>[function <span class="apidocSignatureSpan">consul.Status.prototype.</span>peers (opts, callback)](#apidoc.element.consul.Status.prototype.peers)
- description and source-code
```javascript
peers = function (opts, callback) {
  if (!callback) {
    callback = opts;
    opts = {};
  }

  opts = utils.normalizeKeys(opts);
  opts = utils.defaults(opts, this.consul._defaults);

  var req = {
    name: 'status.peers',
    path: '/status/peers',
  };

  utils.options(req, opts);

  this.consul._get(req, utils.body, callback);
}
```
- example usage
```shell
...
Result

''' json
"127.0.0.1:8300"
'''

<a name="status-peers"></a>
### consul.status.peers(callback)

Returns the current Raft peer set.

Usage

''' javascript
consul.status.peers(function(err, result) {
...
```



# <a name="apidoc.module.consul.Watch"></a>[module consul.Watch](#apidoc.module.consul.Watch)

#### <a name="apidoc.element.consul.Watch.Watch"></a>[function <span class="apidocSignatureSpan">consul.</span>Watch (consul, opts)](#apidoc.element.consul.Watch.Watch)
- description and source-code
```javascript
function Watch(consul, opts) {
  var self = this;

  events.EventEmitter.call(self);

  opts = utils.normalizeKeys(opts);

  var options = utils.normalizeKeys(opts.options || {});
  options = utils.defaults(options, consul._defaults);
  options.wait = options.wait || '30s';
  options.index = options.index || '0';

  self._context = { consul: consul };
  self._options = options;
  self._attempts = 0;
  self._method = opts.method;

  if (typeof opts.method !== 'function') {
    throw errors.Validation('method required');
  }

  process.nextTick(function() { self._run(); });
}
```
- example usage
```shell
...
/**
 * Watch helper.
 */

Consul.meta.watch = { type: 'eventemitter' };

Consul.prototype.watch = function(opts) {
  return new Consul.Watch(this, opts);
};

/**
 * Walk methods
 */

Consul.meta.walk = { type: 'sync' };
...
```

#### <a name="apidoc.element.consul.Watch.super_"></a>[function <span class="apidocSignatureSpan">consul.Watch.</span>super_ ()](#apidoc.element.consul.Watch.super_)
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



# <a name="apidoc.module.consul.Watch.prototype"></a>[module consul.Watch.prototype](#apidoc.module.consul.Watch.prototype)

#### <a name="apidoc.element.consul.Watch.prototype._err"></a>[function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>_err (err, res)](#apidoc.element.consul.Watch.prototype._err)
- description and source-code
```javascript
_err = function (err, res) {
  var self = this;

  if (self._end) return;

  self.emit('error', err, res);

  if (res && res.statusCode === 400) return self.end();

  utils.setTimeoutContext(function() { self._run(); }, self, self._wait());
}
```
- example usage
```shell
...
  path: '/acl/update',
  query: {},
  type: 'json',
  body: {},
};

if (!opts.id) {
  return callback(this.consul._err(errors.Validation('id required'), req));
}

req.body.ID = opts.id;

if (opts.name) req.body.Name = opts.name;
if (opts.type) req.body.Type = opts.type;
if (opts.rules) req.body.Rules = opts.rules;
...
```

#### <a name="apidoc.element.consul.Watch.prototype._run"></a>[function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>_run ()](#apidoc.element.consul.Watch.prototype._run)
- description and source-code
```javascript
_run = function () {
  var self = this;

  if (self._end) return;

  var opts = utils.clone(self._options);
  opts.ctx = self;

  try {
    self._method.call(self._context, opts, function(err, data, res) {
      if (err) {
        return self._err(err, res);
      }

      self._updateTime = +new Date();

      self._attempts = 0;

      var newIndex = res.headers['x-consul-index'];

      if (utils.hasIndexChanged(newIndex, self._options.index)) {
        self._options.index = newIndex;

        self.emit('change', data, res);
      }

      process.nextTick(function() { self._run(); });
    });
  } catch (err) {
    self._err(err);
  }
}
```
- example usage
```shell
...
 ctx.lockWaitTime = self._opts.lockwaittime || DEFAULT_LOCK_WAIT_TIME;
 ctx.lockWaitTimeout = utils.parseDuration(ctx.lockWaitTime) + 1000;
 ctx.lockRetryTime = utils.parseDuration(self._opts.lockretrytime || DEFAULT_LOCK_RETRY_TIME);
 ctx.state = 'session';
 ctx.value = self._opts.value || null;

 process.nextTick(function() {
   self._run(ctx);
 });
};

/**
* Release lock
*/
...
```

#### <a name="apidoc.element.consul.Watch.prototype._wait"></a>[function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>_wait ()](#apidoc.element.consul.Watch.prototype._wait)
- description and source-code
```javascript
_wait = function () {
  return Math.min(Math.pow(2, ++this._attempts), 256) * 100;
}
```
- example usage
```shell
...
Lock.prototype._run = function(ctx) {
if (ctx.end) return;

switch (ctx.state) {
  case 'session':
    return this._session(ctx);
  case 'wait':
    return this._wait(ctx);
  case 'acquire':
    return this._acquire(ctx);
  case 'monitor':
    return this._monitor(ctx);
  default:
    throw new Error('invalid state: ' + ctx.state);
}
...
```

#### <a name="apidoc.element.consul.Watch.prototype.end"></a>[function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>end ()](#apidoc.element.consul.Watch.prototype.end)
- description and source-code
```javascript
end = function () {
  if (this._end) return;
  this._end = true;

  this.emit('cancel');
  this.emit('end');
}
```
- example usage
```shell
...
  console.log('data:', data);
});

watch.on('error', function(err) {
  console.log('error:', err);
});

setTimeout(function() { watch.end(); }, 30 * 1000);
'''

<a name="promise-wrapper"></a>
### Promise Wrapper

''' javascript
var Bluebird = require('bluebird');
...
```

#### <a name="apidoc.element.consul.Watch.prototype.isRunning"></a>[function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>isRunning ()](#apidoc.element.consul.Watch.prototype.isRunning)
- description and source-code
```javascript
isRunning = function () {
  return !this._end;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.Watch.prototype.updateTime"></a>[function <span class="apidocSignatureSpan">consul.Watch.prototype.</span>updateTime ()](#apidoc.element.consul.Watch.prototype.updateTime)
- description and source-code
```javascript
updateTime = function () {
  return this._updateTime;
}
```
- example usage
```shell
...
});

var ttl = ctx.session.ttl && utils.parseDuration(ctx.session.ttl);

// monitor updates
if (ttl) {
  utils.setIntervalContext(function() {
    var time = monitor.updateTime();

    if (time && new Date() - time > ttl + 1000) {
      monitor.end();
    }
  }, ctx, Math.min(1000, ttl));
}
...
```



# <a name="apidoc.module.consul.acl"></a>[module consul.acl](#apidoc.module.consul.acl)

#### <a name="apidoc.element.consul.acl.Acl"></a>[function <span class="apidocSignatureSpan">consul.acl.</span>Acl (consul)](#apidoc.element.consul.acl.Acl)
- description and source-code
```javascript
function Acl(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

  if (defaults) this._defaults = defaults;
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
...
```



# <a name="apidoc.module.consul.agent"></a>[module consul.agent](#apidoc.module.consul.agent)

#### <a name="apidoc.element.consul.agent.Agent"></a>[function <span class="apidocSignatureSpan">consul.agent.</span>Agent (consul)](#apidoc.element.consul.agent.Agent)
- description and source-code
```javascript
function Agent(consul) {
  this.consul = consul;
  this.check = new Agent.Check(consul);
  this.service = new Agent.Service(consul);
}
```
- example usage
```shell
...
  if (defaults) this._defaults = defaults;
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);
...
```



# <a name="apidoc.module.consul.catalog"></a>[module consul.catalog](#apidoc.module.consul.catalog)

#### <a name="apidoc.element.consul.catalog.Catalog"></a>[function <span class="apidocSignatureSpan">consul.catalog.</span>Catalog (consul)](#apidoc.element.consul.catalog.Catalog)
- description and source-code
```javascript
function Catalog(consul) {
  this.consul = consul;
  this.node = new Catalog.Node(consul);
  this.service = new Catalog.Service(consul);
}
```
- example usage
```shell
...
}
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);
...
```



# <a name="apidoc.module.consul.consul"></a>[module consul.consul](#apidoc.module.consul.consul)

#### <a name="apidoc.element.consul.consul.Consul"></a>[function <span class="apidocSignatureSpan">consul.consul.</span>Consul (opts)](#apidoc.element.consul.consul.Consul)
- description and source-code
```javascript
function Consul(opts) {
  if (!(this instanceof Consul)) {
    return new Consul(opts);
  }

  opts = utils.defaults({}, opts);

  if (!opts.baseUrl) {
    opts.baseUrl = (opts.secure ? 'https:' : 'http:') + '//' +
      (opts.host || '127.0.0.1') + ':' +
      (opts.port || '8500') + '/v1';
  }
  opts.name = 'consul';
  opts.type = 'json';

  if (opts.defaults) {
    var rawDefaults = utils.normalizeKeys(opts.defaults);
    var defaults;

    constants.DEFAULT_OPTIONS.forEach(function(key) {
      if (!rawDefaults.hasOwnProperty(key)) return;
      if (!defaults) defaults = {};
      defaults[key] = rawDefaults[key];
    });

    if (defaults) this._defaults = defaults;
  }
  delete opts.defaults;

  papi.Client.call(this, opts);

  this.acl = new Consul.Acl(this);
  this.agent = new Consul.Agent(this);
  this.catalog = new Consul.Catalog(this);
  this.event = new Consul.Event(this);
  this.health = new Consul.Health(this);
  this.kv = new Consul.Kv(this);
  this.query = new Consul.Query(this);
  this.session = new Consul.Session(this);
  this.status = new Consul.Status(this);

  try {
    if (opts.promisify) {
      if (typeof opts.promisify === 'function') {
        papi.tools.promisify(this, opts.promisify);
      } else {
        papi.tools.promisify(this);
      }
    }
  } catch (err) {
    err.message = 'promisify: ' + err.message;
    throw err;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.consul.errors"></a>[module consul.errors](#apidoc.module.consul.errors)

#### <a name="apidoc.element.consul.errors.Consul"></a>[function <span class="apidocSignatureSpan">consul.errors.</span>Consul (message)](#apidoc.element.consul.errors.Consul)
- description and source-code
```javascript
function create(message) {
  var error = message instanceof Error ?
    message :
    new Error(message ? message : undefined);

  error.isConsul = true;

  return error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.errors.Validation"></a>[function <span class="apidocSignatureSpan">consul.errors.</span>Validation (message)](#apidoc.element.consul.errors.Validation)
- description and source-code
```javascript
function validation(message) {
  var error = create(message);

  error.isValidation = true;

  return error;
}
```
- example usage
```shell
...
  path: '/acl/update',
  query: {},
  type: 'json',
  body: {},
};

if (!opts.id) {
  return callback(this.consul._err(errors.Validation('id required'), req));
}

req.body.ID = opts.id;

if (opts.name) req.body.Name = opts.name;
if (opts.type) req.body.Type = opts.type;
if (opts.rules) req.body.Rules = opts.rules;
...
```



# <a name="apidoc.module.consul.event"></a>[module consul.event](#apidoc.module.consul.event)

#### <a name="apidoc.element.consul.event.Event"></a>[function <span class="apidocSignatureSpan">consul.event.</span>Event (consul)](#apidoc.element.consul.event.Event)
- description and source-code
```javascript
function Event(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
delete opts.defaults;

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
...
```



# <a name="apidoc.module.consul.health"></a>[module consul.health](#apidoc.module.consul.health)

#### <a name="apidoc.element.consul.health.Health"></a>[function <span class="apidocSignatureSpan">consul.health.</span>Health (consul)](#apidoc.element.consul.health.Health)
- description and source-code
```javascript
function Health(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
...
```



# <a name="apidoc.module.consul.kv"></a>[module consul.kv](#apidoc.module.consul.kv)

#### <a name="apidoc.element.consul.kv.Kv"></a>[function <span class="apidocSignatureSpan">consul.kv.</span>Kv (consul)](#apidoc.element.consul.kv.Kv)
- description and source-code
```javascript
function Kv(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
papi.Client.call(this, opts);

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
...
```



# <a name="apidoc.module.consul.lock"></a>[module consul.lock](#apidoc.module.consul.lock)

#### <a name="apidoc.element.consul.lock.Lock"></a>[function <span class="apidocSignatureSpan">consul.lock.</span>Lock (consul, opts)](#apidoc.element.consul.lock.Lock)
- description and source-code
```javascript
function Lock(consul, opts) {
  events.EventEmitter.call(this);

  opts = utils.normalizeKeys(opts);

  this.consul = consul;
  this._opts = opts;

  if (opts.session) {
    switch (typeof opts.session) {
      case 'string':
        opts.session = { id: opts.session };
        break;
      case 'object':
        opts.session = utils.normalizeKeys(opts.session);
        break;
      default:
        throw errors.Validation('session must be an object or string');
    }
  } else {
    opts.session = {};
  }

  if (!opts.key) {
    throw errors.Validation('key required');
  } else if (typeof opts.key !== 'string') {
    throw errors.Validation('key must be a string');
  }
}
```
- example usage
```shell
...
/**
 * Lock helper.
 */

Consul.meta.lock = { type: 'eventemitter' };

Consul.prototype.lock = function(opts) {
  return new Consul.Lock(this, opts);
};

/**
 * Watch helper.
 */

Consul.meta.watch = { type: 'eventemitter' };
...
```



# <a name="apidoc.module.consul.query"></a>[module consul.query](#apidoc.module.consul.query)

#### <a name="apidoc.element.consul.query.Query"></a>[function <span class="apidocSignatureSpan">consul.query.</span>Query (consul)](#apidoc.element.consul.query.Query)
- description and source-code
```javascript
function Query(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...

this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
...
```



# <a name="apidoc.module.consul.session"></a>[module consul.session](#apidoc.module.consul.session)

#### <a name="apidoc.element.consul.session.Session"></a>[function <span class="apidocSignatureSpan">consul.session.</span>Session (consul)](#apidoc.element.consul.session.Session)
- description and source-code
```javascript
function Session(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
this.acl = new Consul.Acl(this);
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
    } else {
...
```



# <a name="apidoc.module.consul.status"></a>[module consul.status](#apidoc.module.consul.status)

#### <a name="apidoc.element.consul.status.Status"></a>[function <span class="apidocSignatureSpan">consul.status.</span>Status (consul)](#apidoc.element.consul.status.Status)
- description and source-code
```javascript
function Status(consul) {
  this.consul = consul;
}
```
- example usage
```shell
...
this.agent = new Consul.Agent(this);
this.catalog = new Consul.Catalog(this);
this.event = new Consul.Event(this);
this.health = new Consul.Health(this);
this.kv = new Consul.Kv(this);
this.query = new Consul.Query(this);
this.session = new Consul.Session(this);
this.status = new Consul.Status(this);

try {
  if (opts.promisify) {
    if (typeof opts.promisify === 'function') {
      papi.tools.promisify(this, opts.promisify);
    } else {
      papi.tools.promisify(this);
...
```



# <a name="apidoc.module.consul.super_"></a>[module consul.super_](#apidoc.module.consul.super_)

#### <a name="apidoc.element.consul.super_.super_"></a>[function <span class="apidocSignatureSpan">consul.</span>super_ ()](#apidoc.element.consul.super_.super_)
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



# <a name="apidoc.module.consul.super_.prototype"></a>[module consul.super_.prototype](#apidoc.module.consul.super_.prototype)

#### <a name="apidoc.element.consul.super_.prototype.__create"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>__create (request, next)](#apidoc.element.consul.super_.prototype.__create)
- description and source-code
```javascript
__create = function (request, next) {
  var self = this;

  var opts = request.opts;
  var path = opts.path;

  if (typeof path !== 'string') {
    return next(errors.Validation('path required'));
  }

  var headers = utils.mergeHeaders(self._opts.headers, opts.headers);

  // path
  try {
    path = path.replace(/\{(\w+)\}/g, function(src, dst) {
      if (!opts.params.hasOwnProperty(dst)) {
        throw errors.Validation('missing param: ' + dst);
      }

      var part = opts.params[dst] || '';

      // optionally disable param encoding
      return part.encode === false && part.toString ?
        part.toString() : encodeURIComponent(part);
    });
  } catch (err) {
    return next(err);
  }

  // query
  if (!utils.isEmpty(opts.query)) {
    try {
      path += '?' + self._encode('application/x-www-form-urlencoded',
                                 opts.query).toString();
    } catch (err) {
      return next(err);
    }
  }

  // body
  if (opts.body !== undefined) {
    var mime = constants.MIME_ALIAS[opts.type] ||
      headers['content-type'] ||
      constants.MIME_ALIAS[self._opts.type];

    var isFunction = typeof opts.body === 'function';

    if (isFunction) {
      try {
        request.body = opts.body();
      } catch (err) {
        return next(err);
      }
    } else {
      request.body = opts.body;
    }

    var isBuffer = Buffer.isBuffer(request.body);
    var isStream = utils.isReadableStream(request.body);

    if (!isBuffer && !isStream && !mime) {
      return next(errors.Validation('type required'));
    }

    if (!isBuffer && !isStream) {
      if (self._opts.encoders[mime]) {
        try {
          request.body = this._encode(mime, request.body);
        } catch (err) {
          return next(err);
        }
      } else {
        return next(errors.Codec('type is unknown: ' + mime));
      }
    }

    if (!headers['content-type'] && mime) {
      headers['content-type'] = mime + '; charset=' + constants.CHARSET;
    }

    if (isStream) {
      if (!isFunction) request._retryable = false;
    } else {
      headers['content-length'] = request.body.length;
    }
  } else if (!~constants.EXCLUDE_CONTENT_LENGTH.indexOf(opts.method)) {
    headers['content-length'] = 0;
  }

  // response pipe
  if (opts.pipe) {
    var isPipeFunction = typeof opts.pipe === 'function';

    if (isPipeFunction) {
      try {
        request.pipe = opts.pipe();
      } catch (err) {
        return next(err);
      }
    } else {
      request.pipe = opts.pipe;

      request._retryable = false;
    }

    if (!utils.isWritableStream(request.pipe)) {
      return next(errors.Validation('pipe must be a writable stream'));
    }
  }

  // build http.request options
  request.req = utils.merge(
    utils.pick(self._opts, constants.CLIENT_OPTIONS),
    utils.pick(self._opts.baseUrl, 'auth', 'hostname', 'port', 'path'),
    utils.pick(opts, constants.REQUEST_OPTIONS),
    { headers: headers }
  );

  // append request path to baseUrl
  request.req.path += path;

  // pick http transport
  if (self._opts.baseUrl.protocol === 'https:') {
    request.transport = https;
    if (!request.req.port) request.req.port = 443;
  } else {
    request.transport = http;
    if (!request.req.port) request.req.port = 80;
  }

  if (request.req.auth === null) delete request.req.auth;

  next();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype.__execute"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>__execute (request, next)](#apidoc.element.consul.super_.prototype.__execute)
- description and source-code
```javascript
__execute = function (request, next) {
  var self = this;

  if (request.ctx) {
    if (request.ctx.canceled === true) {
      return next(errors.Validation('ctx already canceled'));
    } else if (request.ctx.finished === true) {
      return next(errors.Validation('ctx already finished'));
    }
  }

  var done = false;

  var opts = request.opts;

  var abort;
  var timeoutId;
  var timeout = opts.hasOwnProperty('timeout') ?
    opts.timeout : self._opts.timeout;

  self._log(['papi', 'request'].concat(opts.tags), request.req);

  var req = request.transport.request(request.req);

  var userAgent = req.getHeader('user-agent');

  if (userAgent === undefined) {
    req.setHeader('user-agent', 'papi/' + meta.version);
  } else if (userAgent === null) {
    req.removeHeader('user-agent');
  }

  req.on('error', function(err) {
    self._log(['papi', 'request', 'error'].concat(opts.tags), err);

    if (done) return;
    done = true;

    if (abort) request.ctx.removeListener('cancel', abort);
    if (timeoutId) clearTimeout(timeoutId);

    request.err = err;
    next();
  });

  if (request.ctx) {
    abort = function() {
      req.abort();
      req.emit('error', errors.Abort('request aborted'));
    };

    request.ctx.once('cancel', abort);
  }

  // set request and absolute timeout
  if (timeout && timeout > 0) {
    timeoutId = setTimeout(function() {
      req.emit('timeout');
      req.abort();
    }, timeout);

    req.setTimeout(timeout);
  }

  req.on('timeout', function(err) {
    self._log(['papi', 'request', 'error', 'timeout'].concat(opts.tags));
    if (err) {
      err = errors.Timeout(err);
    } else {
      err = errors.Timeout('request timed out (' + timeout + 'ms)');
    }
    req.emit('error', err);
  });

  req.on('response', function(res) {
    var chunks = [];
    var bodyLength = 0;

    self._log(['papi', 'response'].concat(opts.tags), {
      method: opts.method,
      path: req.path,
      statusCode: res.statusCode,
      headers: res.headers,
      remoteAddress: res.connection.remoteAddress,
      remotePort: res.connection.remotePort,
    });

    request.res = res;

    if (request.pipe) {
      res.pipe(request.pipe);
    } else {
      res.on('data', function(chunk) {
        chunks.push(chunk);
        bodyLength += chunk.length;
      });
    }

    res.on('end', function() {
      if (done) return;
      done = true;

      if (abort) request.ctx.removeListener('cancel', abort);
      if (timeoutId) clearTimeout(timeoutId);

      // body content mime
      var mime;

      // decode body
      if (bodyLength) {
        res.body = Buffer.concat(chunks, bodyLength);

        // don't decode if user explicitly asks for buffer
        if (!opts.buffer) {
          mime = (res.headers['content-type'] || '').split(';')[0].trim();

          if (self._opts.decoders[mime]) {
            try {
              res.body = self._decode(mime, res.body);
            } catch (err) {
              request.err = err;
              return next();
            }
          }
        }
      }

      // any non-200 is consider an error
      if (Math.floor(res.statusCode / 100) !== 2) {
        var err = errors.Response();

        if (res.body && mime === 'text/plain' && res.body.length < 80) {
          err.message = res.body;
        }

        if (!err.message) {
          if (http.STATUS_CODES[res.statusCode]) {
            err.message = http.STATUS_CODES[res.statusCode].toLowerCase();
          } else {
            err.message = 'request failed: ' + res.statusCode;
          }
        }

        err.statusCode = res.statusCode;

        request.err = err;
      }

      next();
    });
  });

  if (utils.isReadableStream(request.body)) {
    request.body.pipe(req);
  } else {
    req.end(request.body);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype.__push"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>__push (request, name)](#apidoc.element.consul.super_.prototype.__push)
- description and source-code
```javascript
__push = function (request, name) {
  if (this._exts[name]) {
    request._stack.push.apply(request._stack, this._exts[name]);
  }

  if (request.opts && request.opts.exts && request.opts.exts[name]) {
    if (Array.isArray(request.opts.exts[name])) {
      request._stack.push.apply(request._stack, request.opts.exts[name]);
    } else {
      request._stack.push(request.opts.exts[name]);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._decode"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_decode (mime, value)](#apidoc.element.consul.super_.prototype._decode)
- description and source-code
```javascript
_decode = function (mime, value) {
  if (!this._opts.decoders[mime]) {
    throw errors.Codec('unknown decoder: ' + mime);
  }

  try {
    return this._opts.decoders[mime](value);
  } catch (err) {
    err.message = 'decode (' + mime + ') failed: ' + err.message;
    throw errors.Codec(err);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._delete"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_delete (opts)](#apidoc.element.consul.super_.prototype._delete)
- description and source-code
```javascript
_delete = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
...

  if (opts.recurse) req.query.recurse = 'true';

  if (opts.hasOwnProperty('cas')) req.query.cas = opts.cas;

  utils.options(req, opts);

  this.consul._delete(req, utils.empty, callback);
};

Kv.meta.delete = { type: 'alias' };

Kv.prototype.delete = Kv.prototype.del;

/**
...
```

#### <a name="apidoc.element.consul.super_.prototype._encode"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_encode (mime, value)](#apidoc.element.consul.super_.prototype._encode)
- description and source-code
```javascript
_encode = function (mime, value) {
  if (!this._opts.encoders[mime]) {
    throw errors.Codec('unknown encoder: ' + mime);
  }

  try {
    return this._opts.encoders[mime](value);
  } catch (err) {
    err.message = 'encode (' + mime + ') failed: ' + err.message;
    throw errors.Codec(err);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._err"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_err (err, opts)](#apidoc.element.consul.super_.prototype._err)
- description and source-code
```javascript
_err = function (err, opts) {
  if (!err) return err;

  if (!(err instanceof Error)) err = new Error(err);

  if (opts && opts.name) {
    err.message = util.format('%s: %s', opts.name, err.message);
  }

  if (this._opts.name) {
    err.message = util.format('%s: %s', this._opts.name, err.message);
  }

  return err;
}
```
- example usage
```shell
...
  path: '/acl/update',
  query: {},
  type: 'json',
  body: {},
};

if (!opts.id) {
  return callback(this.consul._err(errors.Validation('id required'), req));
}

req.body.ID = opts.id;

if (opts.name) req.body.Name = opts.name;
if (opts.type) req.body.Type = opts.type;
if (opts.rules) req.body.Rules = opts.rules;
...
```

#### <a name="apidoc.element.consul.super_.prototype._ext"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_ext (eventName, callback)](#apidoc.element.consul.super_.prototype._ext)
- description and source-code
```javascript
_ext = function (eventName, callback) {
  if (!eventName || typeof eventName !== 'string') {
    throw this._err(errors.Validation('extension eventName required'));
  }

  if (typeof callback !== 'function') {
    throw this._err(errors.Validation('extension callback required'));
  }

  if (!this._exts[eventName]) this._exts[eventName] = [];

  this._exts[eventName].push(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._get"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_get (opts)](#apidoc.element.consul.super_.prototype._get)
- description and source-code
```javascript
_get = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
...

 if (!opts.id) {
   return callback(this.consul._err(errors.Validation('id required'), req));
 }

 utils.options(req, opts);

 this.consul._get(req, utils.bodyItem, callback);
};

Acl.prototype.get = Acl.prototype.info;

/**
* Creates a new token by cloning an existing token
*/
...
```

#### <a name="apidoc.element.consul.super_.prototype._head"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_head (opts)](#apidoc.element.consul.super_.prototype._head)
- description and source-code
```javascript
_head = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._log"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_log (tags, data)](#apidoc.element.consul.super_.prototype._log)
- description and source-code
```javascript
_log = function (tags, data) {
  return this.emit('log', tags, data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._options"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_options (opts)](#apidoc.element.consul.super_.prototype._options)
- description and source-code
```javascript
_options = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._patch"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_patch (opts)](#apidoc.element.consul.super_.prototype._patch)
- description and source-code
```javascript
_patch = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._plugin"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_plugin (plugin, options)](#apidoc.element.consul.super_.prototype._plugin)
- description and source-code
```javascript
_plugin = function (plugin, options) {
  if (!plugin) {
    throw this._err(errors.Validation('plugin required'));
  }

  if (typeof plugin.register !== 'function') {
    throw this._err(errors.Validation('plugin must have register function'));
  }

  var attributes = plugin.register.attributes;

  if (!attributes) {
    throw this._err(errors.Validation('plugin attributes required'));
  }

  if (!attributes.name) {
    throw this._err(errors.Validation('plugin attributes name required'));
  }

  if (!attributes.version) {
    throw this._err(errors.Validation('plugin attributes version required'));
  }

  return plugin.register(this, options || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.super_.prototype._post"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_post (opts)](#apidoc.element.consul.super_.prototype._post)
- description and source-code
```javascript
_post = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
...
    }
  } catch (err) {
    return callback(this.consul._err(err, req));
  }

  utils.options(req, opts);

  this.consul._post(req, utils.body, callback);
};

/**
 * Gets a given query
 */

Query.prototype.get = function(opts, callback) {
...
```

#### <a name="apidoc.element.consul.super_.prototype._put"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_put (opts)](#apidoc.element.consul.super_.prototype._put)
- description and source-code
```javascript
_put = function (opts) {
  var args;

  if (typeof opts === 'string') {
    opts = { path: opts, method: reqMethod };

    args = Array.prototype.slice.call(arguments);
    args[0] = opts;

    return this._request.apply(this, args);
  } else if (!opts) {
    args = Array.prototype.slice.call(arguments);
    args[0] = {};

    return this._request.apply(this, args);
  }

  opts.method = reqMethod;

  return this._request.apply(this, arguments);
}
```
- example usage
```shell
...

  if (opts.name) req.body.Name = opts.name;
  if (opts.type) req.body.Type = opts.type;
  if (opts.rules) req.body.Rules = opts.rules;

  utils.options(req, opts);

  this.consul._put(req, utils.body, callback);
};

/**
 * Update the policy of a token
 */

Acl.prototype.update = function(opts, callback) {
...
```

#### <a name="apidoc.element.consul.super_.prototype._request"></a>[function <span class="apidocSignatureSpan">consul.super_.prototype.</span>_request (opts)](#apidoc.element.consul.super_.prototype._request)
- description and source-code
```javascript
_request = function (opts) {
  var self = this;

  var request;

  if (this.__request) {
    request = this.__request;
    opts = request.opts;
    self = request._client;
  } else {
    request = {
      _args: Array.prototype.slice.call(arguments),
      _client: this,
      opts: opts,
      state: {},
    };

    if (!opts) opts = request.opts = {};

    if (request._args.length > 1) {
      request._callback = request._args[request._args.length - 1];
    } else {
      return self.emit('error', self._err(
        errors.Validation('callback required'), opts));
    }

    // if ctx is an event emitter we use it to abort requests when done is
    // emitted
    if (opts.ctx instanceof events.EventEmitter) {
      request.ctx = opts.ctx;
    }

    // combine global and request tags
    opts.tags = (opts.tags || []).concat(self._opts.tags);

    // inject request name into tags if not already defined
    if (opts.name && !~opts.tags.indexOf(opts.name)) {
      opts.tags.push(opts.name);
    }

    if (!opts.headers) opts.headers = {};
    if (!opts.params) opts.params = {};
    if (!opts.query) opts.query = {};

    // restart request
    request.retry = function() {
      if (request._retryable === false) {
        throw errors.Validation('request is not retryable');
      }

      self._log(['papi', 'request', 'retry'].concat(request.opts.tags));

      delete request.body;
      delete request.err;
      delete request.req;
      delete request.res;
      delete request.transport;

      self._request.call({ __request: request });
    };

    request._stack = [];

    self.__push(request, 'onCreate');

    request._stack.push(self.__create);

    self.__push(request, 'onRequest');

    request._stack.push(self.__execute);

    self.__push(request, 'onResponse');

    request._stack.push.apply(
      request._stack,
      request._args.slice(1, request._args.length - 1)
    );
  }

  var i = 0;
  function next(err) {
    if (err) return request._callback(self._err(err, opts));

    // middlware can call next(false, args...) to stop middleware
    if (err === false) {
      return request._callback.apply(null,
        Array.prototype.slice.call(arguments, 1));
    }

    var fn = request._stack[i++];
    if (fn) {
      fn.call(self, request, next);
    } else {
      request._callback.call(self, self._err(request.err, opts), request.res);
    }
  }

  next();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.consul.utils"></a>[module consul.utils](#apidoc.module.consul.utils)

#### <a name="apidoc.element.consul.utils.body"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>body (request, next)](#apidoc.element.consul.utils.body)
- description and source-code
```javascript
function body(request, next) {
  if (request.err) return next(false, request.err, undefined, request.res);

  next(false, undefined, request.res.body, request.res);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.utils.bodyItem"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>bodyItem (request, next)](#apidoc.element.consul.utils.bodyItem)
- description and source-code
```javascript
function bodyItem(request, next) {
  if (request.err) return next(false, request.err, undefined, request.res);

  if (request.res.body && request.res.body.length) {
    return next(false, undefined, request.res.body[0], request.res);
  }

  next(false, undefined, undefined, request.res);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.utils.clone"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>clone (src)](#apidoc.element.consul.utils.clone)
- description and source-code
```javascript
function clone(src) {
  var dst = {};

  for (var key in src) {
    if (src.hasOwnProperty(key)) {
      dst[key] = src[key];
    }
  }

  return dst;
}
```
- example usage
```shell
...
 "Name": "Read only",
 "Type": "client",
 "Rules": "{\"key\":{\"\":{\"policy\":\"read\"}}}"
}
'''

<a name="acl-clone"></a>
### consul.acl.clone(options, callback)

Creates a new token by cloning an existing token.

Options

* id (String): token ID
...
```

#### <a name="apidoc.element.consul.utils.createCheck"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>createCheck (src)](#apidoc.element.consul.utils.createCheck)
- description and source-code
```javascript
function createCheck(src) {
  src = normalizeKeys(src);

  var dst = _createServiceCheck(src);

  if (src.name) {
    dst.Name = src.name;
  } else {
    throw new Error('name required');
  }

  if (src.hasOwnProperty('id')) dst.ID = src.id;
  if (src.hasOwnProperty('serviceid')) dst.ServiceID = src.serviceid;

  return dst;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.utils.createServiceCheck"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>createServiceCheck (src)](#apidoc.element.consul.utils.createServiceCheck)
- description and source-code
```javascript
function createServiceCheck(src) {
  return _createServiceCheck(normalizeKeys(src));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.utils.decode"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>decode (value, opts)](#apidoc.element.consul.utils.decode)
- description and source-code
```javascript
function decode(value, opts) {
  if (typeof value !== 'string') return value;
  value = new Buffer(value, 'base64');
  if (!opts || !opts.buffer) value = value.toString();
  return value;
}
```
- example usage
```shell
...

  utils.options(req, opts);

  this.consul._put(req, utils.body, function(err, data, res) {
    if (err) return callback(err, undefined, res);

    if (data.hasOwnProperty('Payload')) {
      data.Payload = utils.decode(data.Payload, { buffer: buffer });
    }

    callback(null, data, res);
  });
};

/**
...
```

#### <a name="apidoc.element.consul.utils.defaults"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>defaults (obj)](#apidoc.element.consul.utils.defaults)
- description and source-code
```javascript
function defaults(obj) {
  if (!obj) obj = {};

  var src;
  for (var i = 0; i < arguments.length; i++) {
    src = arguments[i];
    for (var p in src) {
      if (src.hasOwnProperty(p) && !obj.hasOwnProperty(p)) {
        obj[p] = src[p];
      }
    }
  }

  return obj;
}
```
- example usage
```shell
...
Acl.prototype.create = function(opts, callback) {
if (!callback) {
  callback = opts;
  opts = {};
}

opts = utils.normalizeKeys(opts);
opts = utils.defaults(opts, this.consul._defaults);

var req = {
  name: 'acl.create',
  path: '/acl/create',
  query: {},
  type: 'json',
  body: {},
...
```

#### <a name="apidoc.element.consul.utils.empty"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>empty (request, next)](#apidoc.element.consul.utils.empty)
- description and source-code
```javascript
function empty(request, next) {
  if (request.err) return next(false, request.err, undefined, request.res);

  next(false, undefined, undefined, request.res);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.consul.utils.hasIndexChanged"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>hasIndexChanged (index, prevIndex)](#apidoc.element.consul.utils.hasIndexChanged)
- description and source-code
```javascript
function hasIndexChanged(index, prevIndex) {
  if (typeof index !== 'string' || !index) return false;
  if (typeof prevIndex !== 'string' || !prevIndex) return true;
  return index !== prevIndex;
}
```
- example usage
```shell
...
  // compatible
  if (data.Flags !== +LOCK_FLAG_VALUE) {
    err = errors.Validation('consul: lock: existing key does not match lock use');
    return self._end(ctx, err, res);
  }

  var newIndex = res.headers['x-consul-index'];
  if (utils.hasIndexChanged(newIndex, ctx.index)) ctx.index = newIndex;

  if (data.Session !== ctx.Session) {
    self.emit('retry', { leader: data.Session });
    return retry();
  }
} else if (res.statusCode !== 404) {
  return self._end(ctx, new Error('consul: lock: error getting key'), res);
...
```

#### <a name="apidoc.element.consul.utils.normalizeKeys"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>normalizeKeys (obj)](#apidoc.element.consul.utils.normalizeKeys)
- description and source-code
```javascript
function normalizeKeys(obj) {
  var result = {};

  if (obj) {
    for (var name in obj) {
      if (obj.hasOwnProperty(name)) {
        result[name.replace(/_/g, '').toLowerCase()] = obj[name];
      }
    }
  }

  return result;
}
```
- example usage
```shell
...

Acl.prototype.create = function(opts, callback) {
if (!callback) {
  callback = opts;
  opts = {};
}

opts = utils.normalizeKeys(opts);
opts = utils.defaults(opts, this.consul._defaults);

var req = {
  name: 'acl.create',
  path: '/acl/create',
  query: {},
  type: 'json',
...
```

#### <a name="apidoc.element.consul.utils.options"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>options (req, opts)](#apidoc.element.consul.utils.options)
- description and source-code
```javascript
function options(req, opts) {
  if (!opts) opts = {};

  if (!req.query) req.query = {};

  if (opts.dc) req.query.dc = opts.dc;
  if (opts.wan) req.query.wan = '1';

  if (opts.consistent) {
    req.query.consistent = '1';
  } else if (opts.stale) {
    req.query.stale = '1';
  }

  if (opts.hasOwnProperty('index')) req.query.index = opts.index;
  if (opts.hasOwnProperty('wait')) req.query.wait = opts.wait;
  if (opts.hasOwnProperty('token')) req.query.token = opts.token;

  // papi
  if (opts.hasOwnProperty('ctx')) req.ctx = opts.ctx;
  if (opts.hasOwnProperty('timeout')) req.timeout = opts.timeout;
}
```
- example usage
```shell
...
   body: {},
 };

 if (opts.name) req.body.Name = opts.name;
 if (opts.type) req.body.Type = opts.type;
 if (opts.rules) req.body.Rules = opts.rules;

 utils.options(req, opts);

 this.consul._put(req, utils.body, callback);
};

/**
* Update the policy of a token
*/
...
```

#### <a name="apidoc.element.consul.utils.parseDuration"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>parseDuration (value)](#apidoc.element.consul.utils.parseDuration)
- description and source-code
```javascript
function parseDuration(value) {
  if (typeof value === 'number') return value / 1e6;
  if (typeof value !== 'string') return;

  var n;
  var m = value.match(/^(\d*\.?\d*)$/);

  if (m) {
    n = parseFloat(m[1]);

    if (!isNaN(n)) return n / 1e6;
  }

  m = value.match(/^([\d\.]*)(ns|us|ms|s|m|h)$/);

  if (!m) return;

  n = parseFloat(m[1]);

  if (isNaN(n)) return;

  return n * constants.DURATION_UNITS[m[2]] / 1e6;
}
```
- example usage
```shell
...
var ctx = self._ctx = new events.EventEmitter();

ctx.key = self._opts.key;
ctx.session = utils.clone(self._opts.session);
ctx.index = '0';
ctx.end = false;
ctx.lockWaitTime = self._opts.lockwaittime || DEFAULT_LOCK_WAIT_TIME;
ctx.lockWaitTimeout = utils.parseDuration(ctx.lockWaitTime) + 1000;
ctx.lockRetryTime = utils.parseDuration(self._opts.lockretrytime || DEFAULT_LOCK_RETRY_TIME);
ctx.state = 'session';
ctx.value = self._opts.value || null;

process.nextTick(function() {
  self._run(ctx);
});
...
```

#### <a name="apidoc.element.consul.utils.parseQueryMeta"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>parseQueryMeta (res)](#apidoc.element.consul.utils.parseQueryMeta)
- description and source-code
```javascript
function parseQueryMeta(res) {
  var meta = {};

  if (res && res.headers) {
    if (res.headers['x-consul-index']) {
      meta.LastIndex = res.headers['x-consul-index'];
    }
    if (res.headers['x-consul-lastcontact']) {
      meta.LastContact = parseInt(res.headers['x-consul-lastcontact'], 10);
    }
    if (res.headers['x-consul-knownleader']) {
      meta.KnownLeader = res.headers['x-consul-knownleader'] === 'true';
    }
    if (res.headers['x-consul-translate-addresses']) {
      meta.AddressTranslationEnabled = res.headers['x-consul-translate-addresses'] === 'true';
    }
  }

  return meta;
}
```
- example usage
```shell
...
/**
 * Parse query meta
 */

Consul.meta.parseQueryMeta = { type: 'sync' };

Consul.parseQueryMeta = Consul.prototype.parseQueryMeta = function(res) {
  return utils.parseQueryMeta(res);
};

/**
 * Module exports.
 */

exports.Consul = Consul;
...
```

#### <a name="apidoc.element.consul.utils.setIntervalContext"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>setIntervalContext (fn, ctx, timeout)](#apidoc.element.consul.utils.setIntervalContext)
- description and source-code
```javascript
function setIntervalContext(fn, ctx, timeout) {
  var id;

  var cancel = function() {
    clearInterval(id);
  };

  id = setInterval(function() { fn(); }, timeout);

  ctx.once('cancel', cancel);
}
```
- example usage
```shell
...
  }, self.consul._defaults),
});

var ttl = ctx.session.ttl && utils.parseDuration(ctx.session.ttl);

// monitor updates
if (ttl) {
  utils.setIntervalContext(function() {
    var time = monitor.updateTime();

    if (time && new Date() - time > ttl + 1000) {
      monitor.end();
    }
  }, ctx, Math.min(1000, ttl));
}
...
```

#### <a name="apidoc.element.consul.utils.setTimeoutContext"></a>[function <span class="apidocSignatureSpan">consul.utils.</span>setTimeoutContext (fn, ctx, timeout)](#apidoc.element.consul.utils.setTimeoutContext)
- description and source-code
```javascript
function setTimeoutContext(fn, ctx, timeout) {
  var id;

  var cancel = function() {
    clearTimeout(id);
  };

  id = setTimeout(function() {
    ctx.removeListener('cancel', cancel);

    fn();
  }, timeout);

  ctx.once('cancel', cancel);
}
```
- example usage
```shell
...
 * Wait for non-locked resource
 */

Lock.prototype._wait = function(ctx) {
var self = this;

var retry = function() {
  utils.setTimeoutContext(function() {
    self._run(ctx);
  }, ctx, ctx.lockRetryTime);
};

var opts = utils.defaults({
  key: ctx.key,
  wait: ctx.lockWaitTime,
...
```



# <a name="apidoc.module.consul.watch"></a>[module consul.watch](#apidoc.module.consul.watch)

#### <a name="apidoc.element.consul.watch.Watch"></a>[function <span class="apidocSignatureSpan">consul.watch.</span>Watch (consul, opts)](#apidoc.element.consul.watch.Watch)
- description and source-code
```javascript
function Watch(consul, opts) {
  var self = this;

  events.EventEmitter.call(self);

  opts = utils.normalizeKeys(opts);

  var options = utils.normalizeKeys(opts.options || {});
  options = utils.defaults(options, consul._defaults);
  options.wait = options.wait || '30s';
  options.index = options.index || '0';

  self._context = { consul: consul };
  self._options = options;
  self._attempts = 0;
  self._method = opts.method;

  if (typeof opts.method !== 'function') {
    throw errors.Validation('method required');
  }

  process.nextTick(function() { self._run(); });
}
```
- example usage
```shell
...
/**
 * Watch helper.
 */

Consul.meta.watch = { type: 'eventemitter' };

Consul.prototype.watch = function(opts) {
  return new Consul.Watch(this, opts);
};

/**
 * Walk methods
 */

Consul.meta.walk = { type: 'sync' };
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
