# Changelog

## [1.1.3] - July 27 2019

### Added

- Added keyboard controls for camera movement
- Added a quick tutorial to help new players move the camera
- Added 32 bit support
- Added minigun
- Added revolver
- Added short information page in the main menu

### Fixed

- Fixed full stop inconsistencies in the menus
- Fixed *no collision* being ignored in saved / copied contraptions
- Fixed serialisation bug where stabbing an object and then removing the stabbing object would cause errors
- Fixed bug that would stop the game from launching on certain computers
- Fixed fixed cable rendering bug

### Changed

- Made truck container background more transparent
- Doubled limb breaking treshold
- Changed the look of the fixed cable to make objects behind more visible
- Decreased camera shake from firearms
- Dimmed selection outline
- Selection outline is now hidden on the immediate held object
- Changed the game's default window mode from fullscreen to borderless
- Made crossbow bolts spawnable objects
- Changed Jukebox custom song loading to occur every launch instead of every map load

## [1.1.2] - July 23 2019

### Added

- Added the Abyss map

### Fixed

- Fixed gyrostabiliser light not toggling
    - Fixed the light being magenta instead of blue

## [1.1.1] - July 21 2019

### Added

- Added more splash sound effects
- Added an ship anchor item
- Added the ability to use custom songs in the Jukebox 
    - Put your **.wav** files in the "Jukebox" directory in the root folder of the game
    - Once you have custom songs loaded, the default jukebox songs will be skipped

### Changed

- Changed the colour of the gyroscope light from green to blue
- Changed the motor so that it no longer dies when underwater
- Changed the look of the jukebox
- Lowered strength of the shotgun

### Fixed

- Fixed incorrect underwater rendering of glowing sprites
- Fixed bubbles rendering inside a jukebox
- Minor bugfixes

## [1.1.0] - July 19 2019

### Added

- Added buoyancy physics
- Added a water map

### Changed

- Updated map thumbnails
- Brightened pause menu background
- Doubled firearm maximum distance

### Removed

- The bridge map was removed

### Fixed

- Fixed serialising of propagation wires connected to motors
- Fixed the UI sound being gone after saving something
- Fixed all sound stopping after saving something and only resuming at a timescale event

## [1.0.2] - July 12 2019

### Added

- Added blood decals
- Added wooden struts

### Changed

- Updated thruster particles
- Changed tool wheel to tool bar

### Fixed

- Fixed unassigned wound neighbour
- Fixed small thruster not burning objects
