# Changelog

All notable changes to `phpunit-snapshot-assertions` will be documented in this file

## 4.0.0 - 2019-02-11

*Snapshots generated with `assertMatchesSnapshot` will break when upgrading to this version. The easiest way to upgrade is to ensure your snapshot tests pass, delete your snapshots, upgrade the package, then rerun the tests to generate new snapshots.*

- New snapshot formats when using `assertMatchesSnapshot`: scalars (strings, integers & floats) are serialized to `txt` files, objects & arrays are serialized to `yaml` files
- New `TextDriver` to store snapshots in `txt` files
- New `ObjectDriver` to serialize data to YAML and store snapshots in `yaml` files
- Removed `VarDriver`

## 3.1.1 - 2019-02-10
- Add support for PHPUnit 9 (#86)

## 3.1.0 - 2019-12-02
- Drop support for PHP 7.3

## 3.0.0 - 2019-11-22
- `assertMatchesJsonSnapshot` now supports all JSON serializable objects, and won't convert empty arrays to obejcts anymore

## 2.2.1 - 2019-11-22
- Allow symfony 5 components

## 2.2.0 - 2019-10-23
- Added an `assertMatchesHtmlSnapshot` assertion

## 2.1.3 - 2019-08-07
- Allow recursive mkdir for file snapshots

## 2.1.2 - 2019-03-27
- Less restrictive symfony/yaml version requirement

## 2.1.1 - 2019-03-04
- Fix for json driver

## 2.1.0 - 2019-02-07
- Require PHPUnit 8 & PHP 7.2

## 2.0.0 - 2019-01-29
- Use YAML by default for associative arrays
- Drop PHP 7.0 support, the new constraint is ^7.1
- Drop PHPUnit ^6.5 support, the new constraint is ^7.0

## 1.4.1 - 2019-01-29
- Fix JSON array comparisons

## 1.4.0 - 2019-01-29
- Allow arrays to be serialized to JSON

## 1.3.3 - 2018-12-15
- Fix updating failed file-snapshots

## 1.3.2 - 2018-10-18
- Fix for tests with weird characters

## 1.3.1 - 2018-06-09
- Lowered minimum required PHPUnit version

## 1.3.0 - 2018-05-22
- Only mark test incomplete after every snapshot has been run

## 1.2.3 - 2018-03-15
- Fixed snapshot creation in recursive directories

## 1.2.2 - 2018-02-17
- Support PHP 7.2

## 1.2.1 - 2018-02-02
- Support phpunit ^7.0

## 1.2.0 - 2017-11-29
- Added `assertMatchesFileSnapshot`

## 1.1.1 - 2017-10-11
- Fixed `assertMatchesFileHashSnapshot`

## 1.1.0 - 2017-10-07
- Added `assertMatchesFileHashSnapshot` assertion

## 1.0.2 - 2017-09-11
- Added `example` folder to `.gitattributes`

## 1.0.1 - 2017-06-23
- Fixed expected and actual argument order when making json assertions

## 1.0.0 - 2017-05-29
- Added a reminder how to update snapshots when a snapshot assertion fails

## 0.4.1 - 2017-03-27
- Initial release
