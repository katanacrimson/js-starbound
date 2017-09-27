# js-starbound

## A collection of node.js libraries for working with Starbound files.

js-starbound is a metapackage to help easily work with several types of Starbound files.

Currently provided are the following libraries:

* [SBON](https://github.com/damianb/SBON)
* [SBVJ01](https://github.com/damianb/SBVJ01)
* [SBAsset6](https://github.com/damianb/SBAsset6)
* [StreamPipeline](https://github.com/damianb/StreamPipeline) (dependency of SBAsset6)
* [ConsumableBuffer](https://github.com/damianb/ConsumableBuffer) (dependency of SBON, SBVJ01, SBAsset6)
* [ConsumableFile](https://github.com/damianb/ConsumableFile) (dependency of SBON, SBVJ01, SBAsset6)
* [ExpandingBuffer](https://github.com/damianb/ExpandingBuffer) (dependency of SBON, SBVJ01, SBAsset6)
* [ExpandingFile](https://github.com/damianb/ExpandingFile) (dependency of SBON, SBVJ01, SBAsset6)

### How do I install this library?

Ensure you have at least node.js v7.6+, and then...

``` bash
$ npm i -s damianb/js-starbound
```

### How do I use this library?

In brief:

``` js
'use strict'
const { SBAsset6, SBVJ01, SBON } = require('js-starbound')

// and use SBAsset6, SBVJ01, SBON...etc. all as is documented for each individual module

```