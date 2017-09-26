# CHANGELOG

## js-starbound v1.2.3

##### ExpandingFile v1.0.2

* **Hotfix to correct regression introduced by adding an `fs.access` check when opening a file.**

##### SBVJ01 v2.1.1

* Update deps to pull in hotfix for `ExpandingFile` regression.

## js-starbound v1.2.2

##### SBVJ01 v2.1.0

* **Add support for unversioned SBVJ01 files.**
Magic byte was identified as an indicator of whether or not the file was a versioned entity. Now using the magic byte to identify whether or not to involve a version byte.
* SBVJ01.version is now an optional property and no longer required to save the entity.

##### ConsumableFile v1.0.1

* Add `fs.access` check when opening a file to read it to verify that the file is indeed readable.
* Unit test cleanup.
* Dependency updates.

##### ExpandingFile v1.0.1

* Add `fs.access` check when opening a file to read it to verify that the file is indeed writable.
* Dependency updates.

## js-starbound v1.2.1

##### ExpandingBuffer v1.1.1

* Add support for `ExpandingBuffer.position` for compatibility with `ExpandingFile`.
* Documentation corrections/improvements.

## js-starbound v1.2.0

##### SBVJ01 v2.0.0

* **Implement write functionality for SBVJ01 files.**  Was previously a read-only library for SBVJ01 files.
* Dependency updates.
* Mocha fixes for Windows use.

##### SBAsset6 v1.2.1

* **Hotfix to correct issue where binary files were being corrupted when read.**
No longer converting files read from SBAsset6 archives to strings; we return the Buffer itself and let the consumer decide on what to do with it.

##### SBON v2.0.1

* **Hotfix to correct failures when writing long-length SBON byte sequences, SBON strings, SBON lists, SBON maps.**
Now correctly using varints instead of standard numbers.

## js-starbound v1.1.0

##### SBON v2.0.0

* **Add support for writing SBON.** Was previously only able to read SBON data.

##### ExpandingFile v1.0.0

* Added to `js-starbound`.

##### ExpandingBuffer v1.0.0

* Added to `js-starbound`.

## js-starbound v1.0.0

##### SBVJ01 v1.0.0

* Added to `js-starbound`.

##### SBAsset6 v1.2.0

* Added to `js-starbound`.

##### SBON v1.0.0

* Added to `js-starbound`.

##### ConsumableBuffer v1.0.0

* Added to `js-starbound`.

##### ConsumableFile v1.0.0

* Added to `js-starbound`.