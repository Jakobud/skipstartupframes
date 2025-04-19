# Changelog

All notable changes to the skipstartupframes MAME LUA plugin will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
<!--
The SSF plugin adheres to Semantic Versioning, right?
-->

<!--
Markdown info:

Reference issues and pull requests - Bring up a list of suggested issues and pull requests within the repository by typing #.
Type the issue or pull request number or title to filter the list, and then press either tab or enter to complete the highlighted result.

Ignore Markdown formatting - Put a \ before the markdown character.
-->

<!--
Does Github generate auto-linked issue and pull request numbers on related key entries below when editing this file?
If so, how is that done?
- Can I do it from my forked repo?
- Can you do it in the develop branch?
If not, it is possible to manually link to the issue, commit, or pull request.
- Type # in a comment box, select the desired item, change to preview, copy/paste the link code into CHANGELOG.md.
-->

<!--
*******************************************************************************************************************
*******************************************************************************************************************
For entries that have a Discussion/Issue/BYOAC thread report, do we want to list both that and the commit/pull #?
*******************************************************************************************************************
*******************************************************************************************************************
-->

<!--
Types of changes:
- "Added" for new features.
- "Changed" for changes in existing functionality.
- "Deprecated" for soon-to-be removed features.
- "Removed" for now removed features.
- "Fixed" for any bug fixes.
- "Security" in case of vulnerabilities. 
-->


## [Unreleased]

### Changed

- Updated values in ssf.txt. __.__% checked. (____ of 2927)
<!--
I assume there's no need to link to the pulls or commits for these repetitive ssf.txt update entries.
If anyone wants to see what changed, the compare page is currently linked to the version number here and on the Github release page.
-->

## [2.2.0] - 2025-04-10

### Changed

- Updated values in ssf.txt. 35.26% checked. (1032 of 2927)

## [2.1.0] - 2025-01-16

### Changed

- Updated Readme to reflect vsync limitations.
<!--
Important enough to include?
-->

- Updated values in ssf.txt. 5.88% checked. (172 of 2923)

### Fixed 

- Fixed "Black out screen during startup" and "Mute audio during startup" settings not saving. [Issue #12](https://github.com/Jakobud/skipstartupframes/issues/12).

- Fixed plugin not working with games that have an "_" in the ROMname. [Issue #14](https://github.com/Jakobud/skipstartupframes/issues/14).

## [2.0.0] - 2024-12-15

### Added

- Added optional format to support soft reset (F3) frame numbers. [Discussion #9](https://github.com/Jakobud/skipstartupframes/discussions/9).
<!--
Clarify entry?
Commit/pull #?
-->

- Added Plugin Options Menu lines for `Use alternate frames for a soft reset` and `Soft reset frames`. [Commit ecc9dad](https://github.com/Jakobud/skipstartupframes/commit/ecc9dad7519e5e0d361639a2ac53495132a9256f).
<!--
Clarify entry?
Commit/pull #?
-->

- Added ssf_custom.txt for saving/customizing frame numbers. [Discussion #10](https://github.com/Jakobud/skipstartupframes/discussions/10).
<!--
Clarify entry?
Commit/pull #?
-->

### Changed

- Massive code refactoring, split into modular files. [Commit ee55040](https://github.com/Jakobud/skipstartupframes/commit/ee55040c1d171145b83f443fe9993a28982a4c8b).

- Updated values in ssf.txt.

### Fixed 

- Fixed debug and debug slow motion toggling. [Issue #8](https://github.com/Jakobud/skipstartupframes/issues/8).

## [1.3.0] - 2024-11-20

### Added

- Added Plugin Option Menu item to adjust frames for current game. [Feature suggested in BYOAC forums thread](https://forum.arcadecontrols.com/index.php/topic,169017.msg1775271.html#msg1775271).

- Added Plugin Options Menu Close when ESCAPE is pressed. [Commit 6ae6452](https://github.com/Jakobud/skipstartupframes/commit/6ae64521b8bd34ad3834f533f587e6e179360c81).

- Set ssf.txt to save when exiting a game or exiting MAME. [Commit cf341d6](https://github.com/Jakobud/skipstartupframes/commit/cf341d6dce55d833542c802e82656a85e83431bb).
<!--
Clarify entry?
Commit/pull #?
-->

- Added preservation of frame target for current game when restarting (F3) a game. [Commit cf341d6](https://github.com/Jakobud/skipstartupframes/commit/cf341d6dce55d833542c802e82656a85e83431bb).
<!--
Clarify entry?
Commit/pull #?
-->

- Ensure that frameTarget is always set to zero for non-existent or negative pre-existing values. [Commit 3f50fa5](https://github.com/Jakobud/skipstartupframes/commit/3f50fa50592dcd6cdcb00d5fd40e75a1f5cccd05).
<!--
Important enough to include?
Clarify entry?
-->

### Changed

- Updated values in ssf.txt.

### Fixed

- Value from ssf.txt is loaded anytime a game is started or reset. [Issue #3](https://github.com/Jakobud/skipstartupframes/issues/3).

- Fixed alphabetical order of ssf.txt. [Commit eeddef5](https://github.com/Jakobud/skipstartupframes/commit/eeddef510d2664427369df1a45b7e51db524395f).

## [1.2.0] - 2024-11-20

### Changed

- Updated values in ssf.txt.

## [1.1.0] - 2024-11-13

### Changed

- Improved screen blackout to apply to all screens for multi-screen games. [Commit f9b7b62](https://github.com/Jakobud/skipstartupframes/commit/f9b7b623d5883190c5487305bd0ccb10a0d4dbe2).

### Fixed

- Fixed issue with wrong screen device tag causing a crash. [Issue reported in BYOAC forums thread](https://forum.arcadecontrols.com/index.php/topic,169017.msg1775223.html#msg1775223).

## [1.0.0] - 2024-11-12

### Added

- First release.

[unreleased]: https://github.com/Jakobud/skipstartupframes/compare/v2.2.0...HEAD
<!--
Change unreleased link to point to Develop branch instead of Main?  https://github.com/Jakobud/skipstartupframes/compare/v2.2.0...develop
-->
[2.2.0]: https://github.com/Jakobud/skipstartupframes/compare/v2.1.0...v2.2.0
[2.1.0]: https://github.com/Jakobud/skipstartupframes/compare/v2.0.0...v2.1.0
[2.0.0]: https://github.com/Jakobud/skipstartupframes/compare/v1.3.0...v2.0.0
[1.3.0]: https://github.com/Jakobud/skipstartupframes/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/Jakobud/skipstartupframes/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/Jakobud/skipstartupframes/compare/v1.0.0...v1.1.0
<!--
Change links for 1.1.0 thru 2.2.0 to the release page like 1.0.0 below?  The release pages have the compare link.
-->
[1.0.0]: https://github.com/Jakobud/skipstartupframes/releases/tag/v1.0.0
