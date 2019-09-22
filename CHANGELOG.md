# Changelog

## [1.2.2] - September ?? 2019

### Added
 - Added tips when you open a map
 - Added a message for users who are experiencing low fps that encourages them to switch to discrete mode
 - Added map wide reverb, this makes guns sound much cooler
 - Added a piston item
 - Added a tonne weight
 - Added the Worm Staff
 - Added a television
 - Added a slow motion speed slider in the settings
 - Added little indicator in the _zoom scroll wheel sensitivity_ setting so you can see what you've actually set it to
 - Added the ability to reverse the polarity of the electromagnet
 - Added Lightning tool
    - Hold and swipe across the screen to indicate direction and fire a lightning bolt
### Changed
 - Redid blood decal sprites
 - Redid blood particles
 - Made menu a little clearer
 - The first shot of an automatic weapon is now a little louder
 - Nerfed androids
 - Androids now bleed oil
 - Ultra strength syringe now slightly charges the body
 - Rewrote ragdoll behaviour 
 **THIS BREAKS ALL HUMANS/ANDROIDS IN ANY CONTRAPTION SAVED IN OLDER VERSIONS**
    - Improved performance
    - Improved stability
    - Better active ragdoll posing / animation system
    - Rewrote circulatory system
        - Humans now have a finite amount of blood, any bleeding wound can be lethal
        - Blood pressure is based on how much blood is left in the system and if the heart is functional. Low blood pressure causes a person to become weak and eventually die
    - Fixed many bugs associated with human behaviour
    - Force poses
 - Improved _discrete_ mode
    - Be sure to change your game to _discrete_ for greater performance, especially when you enjoy having way too many objects on screen
 - Updated to Unity 2019
### Fixed
 - Spike not being detected by metal detector
 - Many bugs relevant to humans and androids
 - Fixed exit wound location bug
### Removed
 - Removed short tutorials
 - Tesla coil no longer breaks

## [1.2.1] - August 14 2019

### Added
 - Added a series of detectors to allow for autonomous contraptions
 - Added device that transforms an electrical signal into an activation trigger
 - Added a floodlight
 - Added a wheel
 - Added a basic spike
 - Added a fire extinguisher
 - Maps with ceilings now have large floodlights
 - Human skeletons now light up when electrified
 - Added object-specific options to the context menu
    - Reverse any vehicle
    - Repair or break any vehicle
    - Toggle parking brakes on vehicles
    - Break or mend bones
    - Change the texture of randomly-textured objects
### Changed
 - Increased size of thumbnails to 512x512
 - Improved look of laser pointer beams
 - Clamped strength of fan blades
 - Improved rendering performance
 - Improved physics performance
 - Improved fire propagation performance
 - Barrels now render burnmarks
### Fixed
 - Contraptions with a full stop in their name couldn't be uploaded to the workshop 
 - Fixed incorrect human description
 - Fixed tank shell saving bug
 - Fixed a problem with human legs being too weak
### Removed
 - Grenade is no longer armed when spawned
 - Barrels no longer deform
 - Removed arrow on motorised wheel since every wheel is now reversable

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
