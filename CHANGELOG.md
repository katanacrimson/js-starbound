# CHANGELOG

## js-starbound v2.0.2

### ***ByteAccordion v1.1.3***

* Now handling reads of 0 bytes in length correctly instead of throwing an Error (an empty buffer is returned instead now).

## js-starbound v2.0.1

* `js-starbound` included packages are all using Jenkins for automated testing.
* `js-starbound` included packages all published individually to npm.
* `js-starbound` included packages dependencies reworked slightly to depend on one another as proper packages.

## js-starbound v2.0.0

* `js-starbound` is now using Yarn for dependency management.
* `js-starbound` is now using Jenkins for Continuous Integration (via a private Jenkins server).
* `js-starbound` is now using TypeDoc for documentation.

#### ***SBAsset6 v2.2.0***

* Now using Yarn for dependency management.
* Now using Jenkins for CI.
* Now using TypeDoc for documentation.
* Dependencies updated.
* Now utilizing ByteAccordion to provide StreamPipeline, ExpandingFile, ExpandingBuffer, ConsumableFile, ConsumableBuffer as necessary.

#### ***SBVJ01 v2.3.0***

* Now using Yarn for dependency management.
* Now using Jenkins for CI.
* Now using TypeDoc for documentation.
* Dependencies updated.
* Now utilizing ByteAccordion to provide StreamPipeline, ExpandingFile, ExpandingBuffer, ConsumableFile, ConsumableBuffer as necessary.

#### ***SBON v2.3.0***

* Now using Yarn for dependency management.
* Now using Jenkins for CI.
* Now using TypeDoc for documentation.
* Dependencies updated.
* Now utilizing ByteAccordion to provide StreamPipeline, ExpandingFile, ExpandingBuffer, ConsumableFile, ConsumableBuffer as necessary.

#### ***ByteAccordion v1.1.0***

* Now using Yarn for dependency management.
* Now using Jenkins for CI.
* Now using TypeDoc for documentation.
* Dependencies updated.
* Now includes StreamPipeline, ExpandingFile, ExpandingBuffer, ConsumableFile, ConsumableBuffer.

#### ***StreamPipeline***

* No longer a separate entity; folded into ByteAccordion.

#### ***ExpandingFile***

* No longer a separate entity; folded into ByteAccordion.

#### ***ExpandingBuffer***

* No longer a separate entity; folded into ByteAccordion.

#### ***ConsumableFile***

* No longer a separate entity; folded into ByteAccordion.

#### ***ConsumableBuffer***

* No longer a separate entity; folded into ByteAccordion.

## js-starbound v1.4.0

* `js-starbound` is now completely using TypeScript! All modules now provide definition files and are using tslint for style enforcement.

##### ***SBAsset6 v2.1.0***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***SBVJ01 v2.2.2***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***SBON v2.1.3***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***StreamPipeline v1.1.2***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***ExpandingFile v1.1.1***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***ExpandingBuffer v1.2.1***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***ConsumableFile v1.1.1***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

##### ***ConsumableBuffer v1.1.1***

* **Now using TypeScript.**
* Now providing definition files.
* Now using tslint for style enforcement.
* Removed runtime type guards.

## js-starbound v1.3.1

##### SBAsset6 v2.0.1

* Added `SBAsset6.progress`, an EventEmitter instance, to improve observability of long-running actions such as large pack/unpack operations.

## ***js-starbound v1.3.0***

##### ***SBAsset6 v2.0.0***

* **Added write support for SBAsset6 archive format.** Now able to create and modify SBAsset6 archives!
* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### SBON v2.0.2

* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### SBVJ01 v2.1.2

* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### ***StreamPipeline v1.0.3***

* **Hotfix for failing test; broken check on StreamPipeline.load().** Now correctly(-ish) checking for ExpandingFile instances.
* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### ExpandingFile v1.0.3

* Fix for failing unit test - added a .gitkeep file so a directory would exist when running clean unit tests.
* Corrected some documentation.
* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### ExpandingBuffer v1.1.2

* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### ConsumableFile v1.0.2

* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

##### ConsumableBuffer v1.0.1

* Updated to use standard for code style enforcement.
* Added Travis CI support for automated testing.

## js-starbound v1.2.4

##### ***SBAsset6 1.2.2***

* **Hotfix to correct incorrect parsing of paths specified in filetable.** Now correctly parsing paths via SBON.readString().

##### StreamPipeline v1.0.0

* Added to `js-starbound`.

## js-starbound v1.2.3

##### ***ExpandingFile v1.0.2***

* **Hotfix to correct regression introduced by adding an `fs.access` check when opening a file.**

##### SBVJ01 v2.1.1

* Update deps to pull in hotfix for `ExpandingFile` regression.

## js-starbound v1.2.2

##### ***SBVJ01 v2.1.0***

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

## ***js-starbound v1.2.0***

##### ***SBVJ01 v2.0.0***

* **Implement write functionality for SBVJ01 files.**  Was previously a read-only library for SBVJ01 files.
* Dependency updates.
* Mocha fixes for Windows use.

##### ***SBAsset6 v1.2.1***

* **Hotfix to correct issue where binary files were being corrupted when read.**
No longer converting files read from SBAsset6 archives to strings; we return the Buffer itself and let the consumer decide on what to do with it.

##### ***SBON v2.0.1***

* **Hotfix to correct failures when writing long-length SBON byte sequences, SBON strings, SBON lists, SBON maps.**
Now correctly using varints instead of standard numbers.

## ***js-starbound v1.1.0***

##### ***SBON v2.0.0***

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
