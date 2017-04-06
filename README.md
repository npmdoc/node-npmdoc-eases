# api documentation for  [eases (v1.0.8)](https://github.com/mattdesl/eases)  [![npm package](https://img.shields.io/npm/v/npmdoc-eases.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-eases) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-eases.svg)](https://travis-ci.org/npmdoc/node-npmdoc-eases)
#### grab bag of easing equations

[![NPM](https://nodei.co/npm/eases.png?downloads=true)](https://www.npmjs.com/package/eases)

[![apidoc](https://npmdoc.github.io/node-npmdoc-eases/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-eases_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-eases/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-eases/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-eases/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Matt DesLauriers",
        "email": "dave.des@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/mattdesl/eases/issues"
    },
    "dependencies": {},
    "description": "grab bag of easing equations",
    "devDependencies": {
        "tape": "~2.13.2"
    },
    "directories": {},
    "dist": {
        "shasum": "f1f5069a6b6ed2ea510f9c6110398d63efe9aee6",
        "tarball": "https://registry.npmjs.org/eases/-/eases-1.0.8.tgz"
    },
    "gitHead": "4eb8bc4c7ea4ed98b075c899cb5867461de4330a",
    "homepage": "https://github.com/mattdesl/eases",
    "keywords": [
        "ease",
        "eases",
        "robert",
        "penner",
        "easing",
        "easings",
        "linear",
        "lerp",
        "animation",
        "tween",
        "anim",
        "animations",
        "tweening",
        "tweens",
        "function",
        "functions",
        "expo",
        "quint",
        "quadratic"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mattdesl",
            "email": "dave.des@gmail.com"
        }
    ],
    "name": "eases",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mattdesl/eases.git"
    },
    "scripts": {
        "dev": "beefy demo/index",
        "test": "node test.js"
    },
    "testling": {
        "files": "test.js",
        "browsers": [
            "ie/6..latest",
            "chrome/22..latest",
            "firefox/16..latest",
            "safari/latest",
            "opera/11.0..latest",
            "iphone/6",
            "ipad/6",
            "android-browser/latest"
        ]
    },
    "version": "1.0.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module eases](#apidoc.module.eases)
1.  [function <span class="apidocSignatureSpan">eases.</span>backIn (t)](#apidoc.element.eases.backIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>backInOut (t)](#apidoc.element.eases.backInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>backOut (t)](#apidoc.element.eases.backOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>bounceIn (t)](#apidoc.element.eases.bounceIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>bounceInOut (t)](#apidoc.element.eases.bounceInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>bounceOut (t)](#apidoc.element.eases.bounceOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>circIn (t)](#apidoc.element.eases.circIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>circInOut (t)](#apidoc.element.eases.circInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>circOut (t)](#apidoc.element.eases.circOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>cubicIn (t)](#apidoc.element.eases.cubicIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>cubicInOut (t)](#apidoc.element.eases.cubicInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>cubicOut (t)](#apidoc.element.eases.cubicOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>elasticIn (t)](#apidoc.element.eases.elasticIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>elasticInOut (t)](#apidoc.element.eases.elasticInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>elasticOut (t)](#apidoc.element.eases.elasticOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>expoIn (t)](#apidoc.element.eases.expoIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>expoInOut (t)](#apidoc.element.eases.expoInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>expoOut (t)](#apidoc.element.eases.expoOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>linear (t)](#apidoc.element.eases.linear)
1.  [function <span class="apidocSignatureSpan">eases.</span>quadIn (t)](#apidoc.element.eases.quadIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>quadInOut (t)](#apidoc.element.eases.quadInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>quadOut (t)](#apidoc.element.eases.quadOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>quartIn (t)](#apidoc.element.eases.quartIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>quartInOut (t)](#apidoc.element.eases.quartInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>quartOut (t)](#apidoc.element.eases.quartOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>quintIn (t)](#apidoc.element.eases.quintIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>quintInOut (t)](#apidoc.element.eases.quintInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>quintOut (t)](#apidoc.element.eases.quintOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>sineIn (t)](#apidoc.element.eases.sineIn)
1.  [function <span class="apidocSignatureSpan">eases.</span>sineInOut (t)](#apidoc.element.eases.sineInOut)
1.  [function <span class="apidocSignatureSpan">eases.</span>sineOut (t)](#apidoc.element.eases.sineOut)



# <a name="apidoc.module.eases"></a>[module eases](#apidoc.module.eases)

#### <a name="apidoc.element.eases.backIn"></a>[function <span class="apidocSignatureSpan">eases.</span>backIn (t)](#apidoc.element.eases.backIn)
- description and source-code
```javascript
function backIn(t) {
  var s = 1.70158
  return t * t * ((s + 1) * t - s)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.backInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>backInOut (t)](#apidoc.element.eases.backInOut)
- description and source-code
```javascript
function backInOut(t) {
  var s = 1.70158 * 1.525
  if ((t *= 2) < 1)
    return 0.5 * (t * t * ((s + 1) * t - s))
  return 0.5 * ((t -= 2) * t * ((s + 1) * t + s) + 2)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.backOut"></a>[function <span class="apidocSignatureSpan">eases.</span>backOut (t)](#apidoc.element.eases.backOut)
- description and source-code
```javascript
function backOut(t) {
  var s = 1.70158
  return --t * t * ((s + 1) * t + s) + 1
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.bounceIn"></a>[function <span class="apidocSignatureSpan">eases.</span>bounceIn (t)](#apidoc.element.eases.bounceIn)
- description and source-code
```javascript
function bounceIn(t) {
  return 1.0 - bounceOut(1.0 - t)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.bounceInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>bounceInOut (t)](#apidoc.element.eases.bounceInOut)
- description and source-code
```javascript
function bounceInOut(t) {
  return t < 0.5
    ? 0.5 * (1.0 - bounceOut(1.0 - t * 2.0))
    : 0.5 * bounceOut(t * 2.0 - 1.0) + 0.5
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.bounceOut"></a>[function <span class="apidocSignatureSpan">eases.</span>bounceOut (t)](#apidoc.element.eases.bounceOut)
- description and source-code
```javascript
function bounceOut(t) {
  var a = 4.0 / 11.0
  var b = 8.0 / 11.0
  var c = 9.0 / 10.0

  var ca = 4356.0 / 361.0
  var cb = 35442.0 / 1805.0
  var cc = 16061.0 / 1805.0

  var t2 = t * t

  return t < a
    ? 7.5625 * t2
    : t < b
      ? 9.075 * t2 - 9.9 * t + 3.4
      : t < c
        ? ca * t2 - cb * t + cc
        : 10.8 * t * t - 20.52 * t + 10.72
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.circIn"></a>[function <span class="apidocSignatureSpan">eases.</span>circIn (t)](#apidoc.element.eases.circIn)
- description and source-code
```javascript
function circIn(t) {
  return 1.0 - Math.sqrt(1.0 - t * t)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.circInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>circInOut (t)](#apidoc.element.eases.circInOut)
- description and source-code
```javascript
function circInOut(t) {
  if ((t *= 2) < 1) return -0.5 * (Math.sqrt(1 - t * t) - 1)
  return 0.5 * (Math.sqrt(1 - (t -= 2) * t) + 1)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.circOut"></a>[function <span class="apidocSignatureSpan">eases.</span>circOut (t)](#apidoc.element.eases.circOut)
- description and source-code
```javascript
function circOut(t) {
  return Math.sqrt(1 - ( --t * t ))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.cubicIn"></a>[function <span class="apidocSignatureSpan">eases.</span>cubicIn (t)](#apidoc.element.eases.cubicIn)
- description and source-code
```javascript
function cubicIn(t) {
  return t * t * t
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.cubicInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>cubicInOut (t)](#apidoc.element.eases.cubicInOut)
- description and source-code
```javascript
function cubicInOut(t) {
  return t < 0.5
    ? 4.0 * t * t * t
    : 0.5 * Math.pow(2.0 * t - 2.0, 3.0) + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.cubicOut"></a>[function <span class="apidocSignatureSpan">eases.</span>cubicOut (t)](#apidoc.element.eases.cubicOut)
- description and source-code
```javascript
function cubicOut(t) {
  var f = t - 1.0
  return f * f * f + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.elasticIn"></a>[function <span class="apidocSignatureSpan">eases.</span>elasticIn (t)](#apidoc.element.eases.elasticIn)
- description and source-code
```javascript
function elasticIn(t) {
  return Math.sin(13.0 * t * Math.PI/2) * Math.pow(2.0, 10.0 * (t - 1.0))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.elasticInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>elasticInOut (t)](#apidoc.element.eases.elasticInOut)
- description and source-code
```javascript
function elasticInOut(t) {
  return t < 0.5
    ? 0.5 * Math.sin(+13.0 * Math.PI/2 * 2.0 * t) * Math.pow(2.0, 10.0 * (2.0 * t - 1.0))
    : 0.5 * Math.sin(-13.0 * Math.PI/2 * ((2.0 * t - 1.0) + 1.0)) * Math.pow(2.0, -10.0 * (2.0 * t - 1.0)) + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.elasticOut"></a>[function <span class="apidocSignatureSpan">eases.</span>elasticOut (t)](#apidoc.element.eases.elasticOut)
- description and source-code
```javascript
function elasticOut(t) {
  return Math.sin(-13.0 * (t + 1.0) * Math.PI/2) * Math.pow(2.0, -10.0 * t) + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.expoIn"></a>[function <span class="apidocSignatureSpan">eases.</span>expoIn (t)](#apidoc.element.eases.expoIn)
- description and source-code
```javascript
function expoIn(t) {
  return t === 0.0 ? t : Math.pow(2.0, 10.0 * (t - 1.0))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.expoInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>expoInOut (t)](#apidoc.element.eases.expoInOut)
- description and source-code
```javascript
function expoInOut(t) {
  return (t === 0.0 || t === 1.0)
    ? t
    : t < 0.5
      ? +0.5 * Math.pow(2.0, (20.0 * t) - 10.0)
      : -0.5 * Math.pow(2.0, 10.0 - (t * 20.0)) + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.expoOut"></a>[function <span class="apidocSignatureSpan">eases.</span>expoOut (t)](#apidoc.element.eases.expoOut)
- description and source-code
```javascript
function expoOut(t) {
  return t === 1.0 ? t : 1.0 - Math.pow(2.0, -10.0 * t)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.linear"></a>[function <span class="apidocSignatureSpan">eases.</span>linear (t)](#apidoc.element.eases.linear)
- description and source-code
```javascript
function linear(t) {
  return t
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quadIn"></a>[function <span class="apidocSignatureSpan">eases.</span>quadIn (t)](#apidoc.element.eases.quadIn)
- description and source-code
```javascript
function quadIn(t) {
  return t * t
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quadInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>quadInOut (t)](#apidoc.element.eases.quadInOut)
- description and source-code
```javascript
function quadInOut(t) {
    t /= 0.5
    if (t < 1) return 0.5*t*t
    t--
    return -0.5 * (t*(t-2) - 1)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quadOut"></a>[function <span class="apidocSignatureSpan">eases.</span>quadOut (t)](#apidoc.element.eases.quadOut)
- description and source-code
```javascript
function quadOut(t) {
  return -t * (t - 2.0)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quartIn"></a>[function <span class="apidocSignatureSpan">eases.</span>quartIn (t)](#apidoc.element.eases.quartIn)
- description and source-code
```javascript
function quarticIn(t) {
  return Math.pow(t, 4.0)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quartInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>quartInOut (t)](#apidoc.element.eases.quartInOut)
- description and source-code
```javascript
function quarticInOut(t) {
  return t < 0.5
    ? +8.0 * Math.pow(t, 4.0)
    : -8.0 * Math.pow(t - 1.0, 4.0) + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quartOut"></a>[function <span class="apidocSignatureSpan">eases.</span>quartOut (t)](#apidoc.element.eases.quartOut)
- description and source-code
```javascript
function quarticOut(t) {
  return Math.pow(t - 1.0, 3.0) * (1.0 - t) + 1.0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quintIn"></a>[function <span class="apidocSignatureSpan">eases.</span>quintIn (t)](#apidoc.element.eases.quintIn)
- description and source-code
```javascript
function qinticIn(t) {
  return t * t * t * t * t
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quintInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>quintInOut (t)](#apidoc.element.eases.quintInOut)
- description and source-code
```javascript
function qinticInOut(t) {
    if ( ( t *= 2 ) < 1 ) return 0.5 * t * t * t * t * t
    return 0.5 * ( ( t -= 2 ) * t * t * t * t + 2 )
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.quintOut"></a>[function <span class="apidocSignatureSpan">eases.</span>quintOut (t)](#apidoc.element.eases.quintOut)
- description and source-code
```javascript
function qinticOut(t) {
  return --t * t * t * t * t + 1
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.sineIn"></a>[function <span class="apidocSignatureSpan">eases.</span>sineIn (t)](#apidoc.element.eases.sineIn)
- description and source-code
```javascript
function sineIn(t) {
  var v = Math.cos(t * Math.PI * 0.5)
  if (Math.abs(v) < 1e-14) return 1
  else return 1 - v
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.sineInOut"></a>[function <span class="apidocSignatureSpan">eases.</span>sineInOut (t)](#apidoc.element.eases.sineInOut)
- description and source-code
```javascript
function sineInOut(t) {
  return -0.5 * (Math.cos(Math.PI*t) - 1)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.eases.sineOut"></a>[function <span class="apidocSignatureSpan">eases.</span>sineOut (t)](#apidoc.element.eases.sineOut)
- description and source-code
```javascript
function sineOut(t) {
  return Math.sin(t * Math.PI/2)
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
