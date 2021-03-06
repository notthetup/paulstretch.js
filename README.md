This is a JavaScript implementation - with a few improvements - of *Paul's Extreme Sound Stretch algorithm* (Paulstretch) by [Nasca Octavian PAUL](https://github.com/paulnasca).

Install
===========

Just download the latest build in [dist/](https://github.com/sebpiq/paulstretch.js/tree/master/dist) , and add it to your html page.


Examples
==========
**NB** : not working on Firefox because of a Firefox bug which doesn't allow MediaElementSourceNodes to play audio data from cross-origins with `Access-Control-Allow-Origin: *` (https://bugzilla.mozilla.org/show_bug.cgi?id=937718)

- Example, stretching a sample from a web worker : http://sebpiq.github.io/paulstretch.js/examples/simple/index.html
- More fun example, creating drones with tracks from SoundCloud : http://sebpiq.github.io/paulstretch.js/examples/stretched-and-droned/dist/index.html

Run tests
==============

Tests are written with mocha.

```
mocha -t 15000
```

Build
=======

```
npm install
browserify index.js > dist/paulstretch.js
```
