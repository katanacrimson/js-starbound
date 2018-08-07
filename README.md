# js-starbound

## A collection of node.js libraries for working with Starbound files.

js-starbound is a metapackage to help easily work with several types of Starbound files.

Currently provided are the following libraries:

* [SBON](https://github.com/damianb/SBON)
* [SBVJ01](https://github.com/damianb/SBVJ01)
* [SBAsset6](https://github.com/damianb/SBAsset6)
* [ByteAccordion](https://github.com/damianb/ByteAccordion) (dependency of SBON, SBVJ01, SBAsset6)

### How do I install this library?

Ensure you have at least node.js v7.6+, and then...

``` bash
$ yarn add js-starbound
```

### How do I use this library?

In brief:

``` js
'use strict'
const { SBAsset6, SBVJ01, SBON } = require('js-starbound')

// and use SBAsset6, SBVJ01, SBON...etc. all as is documented for each individual module

```

Documentation is available here:

* [SBON documentation](https://damianb.github.io/SBON)
* [SBVJ01 documentation](https://damianb.github.io/SBVJ01)
* [SBAsset6 documentation](https://damianb.github.io/SBAsset6/)
* [ByteAccordion documentation](https://damianb.github.io/ByteAccordion)
