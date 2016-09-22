# DiabolicUI Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) 
and this project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased] 2016-09-22
### Added
- Added a new large, square semi-transparent Minimap in true Diablo III style.
- Added NamePlates.
- Added group frames.
- Added auras on the Target frame.
- Added an artifact power display, visible as an XP bar when at character level 110, or as part of the XP tooltip when leveling from 101 to 109.

### Changed
- Sidebars are now only visible for a short duration.
- Health values are visible at all times on the Target Frame now, making it far easier to decide what kind of mob or opponent you are currently facing.
- Warnings and quest objective updates are now displayed more centered, closer to the character. 
- The Game Menu (Esc) centers itself vertically upon display now, making it centered regardless of number of buttons or game client version.

### Fixed
- Fixed a bug where the chat bubbles sometimes would bug out if other addons had added child frames to the WorldFrame.

### Removed
- Removed the old, round Minimap that pretty much was just a slightly reskinned version of the Minimap from Goldpaw's UI. 
- Removed the Blizzard buff and debuff displays.
- Removed the Blizzard group frames.

## [1.0.21] 2016-07-24
### Added
- Added zhTW locale by 公孟一文.

### Fixed
- Fixed number abbreviations on the XP bar for zhCN clients.

## [1.0.20] 2016-07-23
### Added
- Added zhCN entry for the stance button tooltip text.

### Changed
- Updated combo points for Rogues in Legion.

## [1.0.19] 2016-07-21
### Fixed
- Fixed some scaling issues in the custom popups.
- Fixed a problem related to figuring out the graphics resolution when UI scaling was enabled in Legion.

## [1.0.18] 2016-07-20
### Added
- Garrison Minimap button is back.
- Added the stance bar button's tooltip text to the enUS locale.
- Added better number abbreviations for zhCN clients.
- Added zhCN localization by 公孟一文.

### Fixed
- Fixed the mirrortimers and timertrackers. turns out blizzard had changed the names and keys of some of the textures.
- Fixed a tooltip bug when hovering over the stance button.
- Attempted to fix a bug that would occur when other addons used blizzard's TimerTracker system.
- Fixed a tooltip incompatibility with the addon SavedInstances.
- Fixed some problems with the locale handler that would prevent other locales than enUS from functioning.
- Fixed the "big bar in the middle of the screen" bug.
- Fixed an issue that would display a number instead of the red error messages on-screen.
- Fixed the zone ability button.

### Changed
- Bumped interface version to 7.0.3.

## [1.0.17] 2016-07-18
### Fixed
- Fixed a localization bug that would cause pre-Cata clients to malfunction if the UI scale was "incorrect".

## [1.0.16] 2016-07-17
### Added
- Added a popup to request whether or not you prefer to have the main chat window automatically sized and positioned.
- Added the chat commands "/diabolic autoscale", "/diabolic autoposition" and "/diabolic resetsetup".

## [1.0.15] 2016-07-16
### Changed
- Toned down the glare on the minimap overlay texture.
- Added frequent updates for unitframes whose unit didn't fire in events, such as ToT.

### Fixed
- Fixed a weird bug that sometimes would occur in the unitframe threat element.

### Removed
- Removed some debug output from the actionbar module that would show up at the start of pet battles
- Removed the annoying green paw texture that would appear on pet battle chat output frames

## [1.0.14] 2016-07-15
### Added
- Added stack size / spell charges to the actionbuttons.
- Added more updates to ToT unit names.

### Changed
- Moved the player's alternate power down, as it often was in the way of the target frame (for example when the blood moon event was active).

### Fixed
- Fixed action keybind in pet battles.

## [1.0.13] 2016-07-14
### Fixed
- Trying to work around a nil bug in the chat window module related to the chat icons. Unable to reproduce it so far, though.

## [1.0.12] 2016-07-13
### Added
- Added combopoints and anticipation.

### Changed
- Doubled the brightness of the threat texture.

### Removed
- Removed the autominimizing of the quest tracker in combat, as this was causing a taint if the user moved from one subzone to another while having quest objectives visible on the WorldMap and opening it. Now THAT took some time to figure out!

## [1.0.11] 2016-07-12
### Added
- Added threat coloring for all existing units with the exception of the player (that's coming later!).

### Changed
- Moved the durability frame, ghost release frame and vehicle seat indicators.
 
### Fixed
- Fixed issues that prevented new buttons in the stance bar from being clicked when learning new forms or changing talent specialization.
- Updated the Warrior action paging, which seems to have been wrong. New abilities will properly appear on the action bar after this change. 
- Fixed a typo that caused the UI not to load.


## [1.0.10] 2016-07-11
### Added
- Added some temporary statusbar texts for the targetframe and player orbs.

### Changed
- Restyled and repositioned the ExtraActionButton1 and the Draenor Zone ability button.

## [1.0.9] 2016-07-9
### Changed
- Stance (and other) buttons should now properly get a gold border to indicate when they are checked.

### Fixed
- Fixed an issue that would produce a bug if more than one mirrortimer (breath, fatigue, etc) was visible on-screen at once. Also adjusted the coloring to be darker and easier to see.

## [1.0.8] 2016-07-8
### Changed
- Moved the mirrortimer (breath, fatigue, feign death etc) slightly downwards, to make room for the upcoming targetframe auras.
- Moved the warning text ("You can't do that yet" etc) slightly down, to not be in the way of the mirror timer or the target frame.
- Slightly lowered the padding between the buttons on the side bars, pet bar and stance bar.

### Fixed
- Fixed a problem with the actionbutton overlay glows.

## [1.0.7] 2016-07-7
### Added
- Added a stance bar...'ish.

### Fixed
- Fixed a bug in the tracker module that would sometimes taint the worldmap's POI buttons if the worldmap was opened during combat. 
- Fixed a bug that would sometimes cause the focus frame powerbar to become stupid long instead of disappearing.

## [1.0.6] 2016-07-6
### Added
- Added MoveAnything's game menu button to our styled game menu. I highly recommend NOT using MoveAnything, though, as it causes taint and breaks UI and game functionality.

## [1.0.5] 2016-07-5
### Fixed
- Fixed an issue in Legion/WoD where the focus frame wouldn't reposition itself when the pet frame was shown.
- Fixed an issue in Legion where the castbar texture would be pure green, instead of light transparent white.

## [1.0.4] 2016-07-4
### Added
- Added ToT and Focus unitframes.

### Changed
- Chat should be visible for 15 seconds before fading, up from 5.

### Fixed
- Fixed some issues with the unitframe castbars where they sometime wouldn't update properly.
- Fixed a framelevel issue with the unitframe castbars that would render them above their border.
- Fixed a problem that sometimes would occur with female unitframe portraits.
- Fixed an issue where the chat window module would disable itself if Prat-3.0 was in the addon list, even if it wasn't enabled.

## [1.0.3] 2016-07-2
### Added
- Added a pet action bar.

### Changed
- Adjusted how the side bars resize and move themselves.
- Made the actionbar menu's backdrop darker, to make it less confusing when shown over an open quest tracker.
- All unitframe elements (like the portraits) should now be updated also when first shown.

### Fixed
- Fixed a bug that would make it impossible to dismiss or rename a pet through its unitframe after a /reload.

## [1.0.2] 2016-06-23
### Added
- Added the XP bar.
- Added some methods to the custom StatusBar object to accomodate the new XP bar.

### Changed
- Changed the shadow on the chat font to match the UIs general light direction.

### Fixed
- Removed some debugging output that would appear when clicking on the chat button with the mouse.


## [1.0.1] 2016-06-22
### Added
- The FriendsMicroButton is now forcefully hidden.

### Changed
- Updated the readme file.
- Chat module disabled if Prat-3.0 is loaded.
- Reverted the build number used to recognize the Legion expansion to a lower value.

### Fixed
- Fixed an issue where the chat button would sometimes become disabled after the input box was automatically hidden in classic style mode.
- The "canexitvehicle" macro option doesn't exist before MoP.
- Settings should now save properly between sessions for all clients.

### Removed
- Removed flash animations from chat bubbles, as this was causing client crashes for some users.

## [1.0.0] 2016-06-21
- Initial commit.
