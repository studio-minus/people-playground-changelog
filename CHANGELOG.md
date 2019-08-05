# Changelog

## [1.2.0] - August 5 2019

### Added
 - Added Steam Workshop support
 - Added the ability to delete contraptions
 - Added the Beam Rifle
 - Added a giant hovering fan
 - Added mini thruster
 - Added hammer
 - Syringes now also shatter when near an explosion
 - The ability for ragdolls to hold weapons and such:
    - Activate the lower arm of a ragdoll to make it pick up the nearest holdable object
    - Some objects have multiple points to grip
### Changed
- Increased drowning time to 120 seconds
- Increased base strength of the electromagnet
- Increased minigun recoil
- Improved look of sentry turret laser
- Made ragdoll arms a little weaker
- Improved save thumbnail rendering
### Fixed
 - Fixed thruster sound bug
 - Fixed water splash hitbox on *Sea*
 - Revolvers no longer eject shells
 - Fixed not being able to move using keys in paused mode
 - Fixed the revolver ignoring water drag
 - Fixed *no collision* not properly keeping its state after serialisation
 - Fixed joints not keeping their distance occasionally after loading / pasting 
 - Fixed issues with control rebinding in the pause menu
 - Fixed bug to do with water splashes and firearms
### Removed
 - Ragdolls no longer ignite when activated
 - Removed shockwave warping
 - Removed random factor in propagation wire delay
 - Removed ambient sounds

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
