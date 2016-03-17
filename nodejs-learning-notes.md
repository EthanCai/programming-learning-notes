# Books

- [Node入门](http://www.nodebeginner.org/index-zh-cn.html)


# Resources

工具：

- [NPM](https://www.npmjs.com/)
- [CNPM](http://cnpmjs.org/)

文档：

- [NodeJs官网](https://nodejs.org/)
- [ECMAScript 2015 (ES6) in Node.js](https://nodejs.org/en/docs/es6/)
- [Tools and techniques we use at Joyent to operate Node.js in production](https://www.joyent.com/developers/node)

社区：

- [CNode](https://cnodejs.org/)

企业级Node:

- [Node Source](https://nodesource.com/)

--------------------------------

# Basic Projects

参考：

- [Awesome NodeJs](https://github.com/sindresorhus/awesome-nodejs)

## Related JS Language

- [TypeScript](http://www.typescriptlang.org/)

## Compiler

- [node-gyp](https://github.com/nodejs/node-gyp): Node.js native add-on build tool.
- [Babel](https://babeljs.io/): Babel is a JavaScript compiler.
- [asm.js](http://asmjs.org/)
- [Jison](http://zaach.github.io/jison/)
- [ES6 Module Transpiler](http://esnext.github.io/es6-module-transpiler/): ES6 Module Transpiler is a JavaScript library for converting JavaScript files written using the ES6 draft specification module syntax for use in existing JavaScript environments.

## Runtime

- [Alinode](http://alinode.aliyun.com/): alinode 是阿里云出品的 Node.js 应用服务解决方案，是一套基于社区 Node 改进的运行时环境和服务平台。在社区的基础上我们内建了强大的支持功能，帮助开发者迅速洞见性能细节，快速定位疑难杂症，直探问题根源。
- [Alinode Node Profiler](http://profiler.alinode.aliyun.com/): Node Profiler是一款JavaScript的性能调优工具，它不仅知道您的哪些代码慢，还知道为什么慢，能更深度地洞悉性能问题所在

## Package Manager

- [NPM](https://www.npmjs.com/)
- [Bower](http://bower.io/)

## Module Loader

- [RequireJS](http://requirejs.org/)
- [Sea.js](http://seajs.org/docs/)
- [SystemJS](https://github.com/systemjs/systemjs)
- [Webpack](https://webpack.github.io/)
    - [Webpack-howto](https://github.com/petehunt/webpack-howto)
- [Browsify](http://browserify.org/)

## Build & Scaffolding

- [Grunt](http://gruntjs.com/)
- [Gulp](http://gulpjs.com/)
    - [SlushJS](http://slushjs.github.io/#/): The streaming scaffolding system. Gulp as a replacement for Yeoman
- [Yeoman](http://yeoman.io/)

## Documentation

- [JSDoc](http://usejsdoc.org/)

## Debug

- [node-inspector](https://github.com/node-inspector/node-inspector): Node.js debugger based on Blink Developer Tools
- [Debug](https://github.com/visionmedia/debug): tiny node.js & browser debugging utility for your libraries and applications
- [devtool](https://github.com/Jam3/devtool): runs Node.js programs through Chromium DevTools

## Log

- [Winston](https://github.com/winstonjs/winston)
- [log4js-node](https://github.com/nomiddlename/log4js-node)

## Test

- [PhantomJS](http://phantomjs.org/): PhantomJS is a headless WebKit scriptable with a JavaScript API. It has fast and native support for various web standards: DOM handling, CSS selector, JSON, Canvas, and SVG.
- [Mocha](http://mochajs.org/): Mocha is a feature-rich JavaScript test framework running on Node.js and the browser, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases.
- [Chai](http://chaijs.com/): Chai is a BDD / TDD assertion library for node and the browser that can be delightfully paired with any javascript testing framework.
- [jasmine](https://github.com/jasmine/jasmine): DOM-less simple JavaScript testing framework
- [Supertest](https://visionmedia.github.com/superagent/): Super Agent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!
- [Frisby.js](http://frisbyjs.com/docs/api/): Frisby is a REST API testing framework built on node.js and Jasmine that makes testing API endpoints easy, fast, and fun.  
- [Vows](https://github.com/vowsjs/vows): Asynchronous BDD & continuous testing for node.js
- [Istanbul](https://github.com/gotwarlost/istanbul): Yet another JS code coverage tool that computes statement, line, function and branch coverage with module loader hooks to transparently add coverage when running tests. Supports all JS coverage use cases including unit tests, server side functional tests and browser tests. Built for scale.
- [Should.js](http://shouldjs.github.io/): BDD style assertions for node.js -- test framework agnostic

## Network

- [Request](https://github.com/request/request): Simplified HTTP request client
    - [Request-promise](https://github.com/request/request-promise)

## RPC

- [DNode](https://github.com/substack/dnode): dnode is an asynchronous rpc system for node.js that lets you call remote functions.

## Basic Libs

- [Immuable.js](http://facebook.github.io/immutable-js/): Immutable collections for JavaScript
- [lodash](https://lodash.com/): A modern JavaScript utility library delivering modularity, performance, & extras.

## Websocket

- [socket.io](http://socket.io/): Socket.IO enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed.
- [socket.js](https://github.com/boyers/socket.js): A realtime communication framework for Node.js.

## Async & Promise

- [bluebird](http://bluebirdjs.com/docs/getting-started.html)
- [Q](http://documentup.com/kriskowal/q)
- [When](https://github.com/cujojs/when)
- [Async](https://github.com/caolan/async)

## Concurrency

- [fibjs](https://github.com/xicilion/fibjs): fibjs 是一个建立在 Google v8 JavaScript 引擎基础上的应用服务器开发框架，不同于 node.js，fibjs 采用 fiber 解决 v8 引擎的多路复用，并通过大量 c++ 组件，将重负荷运算委托给后台线程，释放 v8 线程，争取更大的并发时间。
- [node-fibers](https://github.com/laverdet/node-fibers): Fiber/coroutine support for v8 and node.
- [node-webworker](https://github.com/pgriess/node-webworker): node-webworkers is an implementation of the Web Workers API for node.js.

## Terminal

- [yargs](https://github.com/yargs/yargs): yargs the modern, pirate-themed successor to optimist.
- [minimist](https://github.com/substack/minimist): parse argument options
- [Optimist](https://github.com/substack/node-optimist): Light-weight option parsing for node.js

## Yaml

- [js-yaml](https://github.com/nodeca/js-yaml): JavaScript YAML parser and dumper. Very fast.

## Stream

- [node-trumpet](https://github.com/substack/node-trumpet): parse and transform streaming html using css selectors
- [csv-stream](https://github.com/klaemo/csv-stream): Streaming CSV Parser for Node. Small and made entirely out of streams.
- [event-stream](https://github.com/dominictarr/event-stream): EvJavaScript YAML parser and dumper. Very fast.entStream is like functional programming meets IO
- [JSONStream](https://github.com/dominictarr/JSONStream): rawStream.pipe(JSONStream.parse()).pipe(streamOfObjects)

## Shim

- [es6-shim](https://github.com/paulmillr/es6-shim)
- [shimmer](https://github.com/othiym23/shimmer)

## Web Framework

- [ExpressJS](http://expressjs.com/)
    - [node-toobusy](https://github.com/lloyd/node-toobusy): Build Node.JS servers that don't fall over.
- [Koa](http://koajs.com/)
- [Connect](https://github.com/senchalabs/connect): Express的前身
- [Micro](https://github.com/zeithq/micro): Async HTTP microservices

## Message Queue & Job Queue

- [Kue](https://github.com/Automattic/kue): Kue is a priority job queue backed by redis, built for node.js.

## Job Schedule

- [node-schedule](https://github.com/node-schedule/node-schedule): A cron-like and not-cron-like job scheduler for Node.
- [node-cron](https://github.com/ncb000gt/node-cron): Cron for NodeJS.
- [Agenda](https://github.com/rschmukler/agenda): Lightweight job scheduling for node
- [Later](https://github.com/bunkat/later): A javascript library for defining recurring schedules and calculating future (or past) occurrences for them. Includes support for using English phrases and Cron schedules. Works in Node and in the browser.

## Desktop

- [Elctron](http://electron.atom.io/): Build cross platform desktop apps with web technologies
- [NW.js](http://nwjs.io/): NW.js (previously known as node-webkit) lets you call all Node.js modules directly from DOM and enables a new way of writing applications with all Web technologies.
- [slimerjs](https://github.com/laurentj/slimerjs)
- [node-qt](https://github.com/arturadib/node-qt): C++ Qt bindings for Node.js
- [nativefier](https://github.com/jiahaog/nativefier): Nativefier is a command line tool that allows you to easily create a desktop application for any web site with succinct and minimal configuration.

## Process Supervisor

- [PM2](https://github.com/Unitech/pm2): Production process manager for Node.js applications with a built-in load balancer https://app.keymetrics.io/
- [Nodemon](http://nodemon.io/): Nodemon is a utility that will monitor for any changes in your source and automatically restart your server. **Perfect for development.**

## App

- [Soundnode](https://github.com/Soundnode/soundnode-app): Soundnode App is an Open-Source project to support Soundcloud for desktop Mac, Windows, and Linux. It's built with NW.js, Node.js, Angular.js, and it uses the Soundcloud API.

## Tools

- [Browsersync](https://browsersync.io/): Time-saving synchronised browser testing.

## Others

- [JXCore](http://jxcore.com/home/): JXcore extends Node.JS™ with additional features for developing mobile and embedded applications using JavaScript and leveraging the Node ecosystem.
- [NodeCG](http://nodecg.com/): NodeCG is a broadcast graphics framework and application. It is primarily aimed at Twitch broadcasters using Open Broadcaster Software, but is usable in any environment that can render HTML, including CasparCG.
- [mjml](https://mjml.io/): MJML is a markup language designed to reduce the pain of coding a responsive email.


--------------------------------

# FAQ
