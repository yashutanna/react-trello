# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.2.0] - 2019-07-20

### Added

* Availability to hide Add Card button for specific lane
* Internationalization support (property `t` and `lang`)
* Russian translation
* Dependency Injection mechanisim for all components customization 
  (property `components`)
* Add `onCardMoveAcrossLanes` handler property, called when a card is moved across lanes
* Add `onDeleteLane` handler property
* Add `laneStyle` property
* Add `editLaneTitle` and `onLaneUpdate` props (availability to inline edit lane
  title)

### Improvements

* Removed CSS style hardcoding (except `react-popover`)
* Upgrade dev dependencies and remove unnecessary pkgs
* Suppress debug prints in tests
* Add babel-plugin-module-resolver to root as ./src
* Removed `react-popover`'s CSS classes. 


### Fixes

* [#203] fixes Cannot drop a card near the bottom of a lane
* [#205] fix argument names in handleLaneDragEnd
* [#201] Fixed Warning: Failed prop type by replacing `react-popover` with `react-popopo`

### Breaking changes

* Removed props `addLaneTitle` and `addCardTitle`. Use `t('Add another lane')` and `t('Click to add card')` instead of it.
* Removed props `customLaneHeader`, `newCardTemplate`, `newLaneTemplate`, `customCardLayout`. Use `components` property instead of it.

Refer [upgrade instructions](UPGRADE.md) to migrate to new version.

## [0.0.0] - [2.1.4]

Lookin into `git log`
