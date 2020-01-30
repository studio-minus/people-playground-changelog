# Changelog

## [1.3] - January 30 2020
### Added
   - A single extra firework variant
   - A set of bells ranging from C4 to C5
   - Structural metal pole thing
   - Siren
   - Propagation wire glows when an activation travels through it
   - Resizing
      - Right click an object, select resize. Two handles will appear, one for each axis.
      - Hold shift (or what you have assigned to "rotate faster") to resize in both axes simultaneously.
### Changed
   - The majority of all machinery is now destructable and will generally cease all function when destroyed
   - Behaviour of aerodynamic objects
   - General Purpose Bomb is now aerodynamic
   - Atom Bomb is now aerodynamic
   - Intensity of plate debris rotational force
   - Cathode lights will now shatter when hit with the Beam Rifle and explosions
   - Piston textures
   - Cathode light texture
   - Car textures
   - Barrel texture
   - Lagbox is now gray to indicate its actually made of metal
   - Desaturated blood
   - Context menu has a scrollbar
   - Propagation wire is thinner and looks different
   - Metronomes no longer burn when energy flows through
   - Increased maximum double click time for map thumbnails
   - Versioning will from now on go 1.3 -> 1.4 -> 1.5 and so on
### Fixed
   - Infinite fireworks activation
   - Incorrect cathode light weightlessness effect position 
   - Incorrect broken plate highlight
   - Incorrect broken plate spawn position
   - Giant wooden bowl not looking burnt after being burnt
   - Weightless gyroscope stabiliser no longer goes haywire
   - Disassembler muzzle flash is no longer gigantic when weightless
   - Canceling saving a contraption is no longer broken
   - You can once again pan while hovering over the toybox panel 
### Removed
   - Firearms no longer create a pulse explosion at their muzzle when fired

## [1.2.7] - December 26 2019
### Added
   - Laser receiver
   - Silver atom bomb texture alternative
   - Text display item
   - General purpose bomb
   - Added plates
   - Added a table
   - And a chair too
   - Stun weapon
   - Fireworks
   - Bowling pin
   - Bowling ball
   - Void map
   - Snowy map
   - Flat bit at the top of Slanted
   - You can double click map thumbnails to load them
   - Blaster bolts now push reflective objects away too
### Changed
   - Replaced "pain" meter with an oxygen meter in the inspector
   - Halved drown time (from 4 to 2 minutes)
   - Decreased chance of losing consciousness on impact
   - Halved water impact damage
   - Abyss thumbnail
   - Normal handgrenades are now less powerful
   - Blaster impact
   - Tank texture
   - Wooden pole texture
   - Button texture
   - Made context menu a little bit smaller
   - Certain UI colours
   - Muzzle flash
   - Generators make less noise
   - Humanoids are now always of equal weight, no matter their height
### Fixed
   - Drowning
   - Bugs to do with crushing & decimation
   - Elimination of tribulation animation synchronisation
   - Rendering optimisation
   - General optimisation
   - Buttons are no longer made of plastic
   - Laser turret serialisation

## [1.2.6] - November 17 2019
### Added
   - Lagbox
   - Cathode lights
   - Laser sentry turret
   - Limb status view
   - Limb crush sensitivity setting
   - F1 opens control screen
   - Added an option for detectors to only trigger on detection, instead of triggering on undetection as well
   - Limb status (toggle with _S_ by default)
   - Detailed inspection of limbs (right click a limb, select _Inspect_)
      - Attempts to combine all information of selected limbs (from different people as well) and display useful information regarding all of them.
   - Some more ambience
### Changed
   - Tank fire sound
   - Humans don't paint the floor with blood when they're drained
   - Firearm damage is now affected by distance
   - Firearms are more powerful at point blank range
   - Increased global bullet speed
   - Halved firearm impact force
   - Decreased bullet speed and damage of the M1
   - Clamped impact particle sizes
   - Slight blue tint
   - Increased health of certain limbs
### Fixed
   - Major firearm ballistics model bugs (especially exit wounds registration)
   - Minor crushed limb bugs
   - Dismembered limbs reacting to fire
   - Damaged androids not sparking anymore after 1.2.2
   - A few spelling errors
   - Scherbenwerfer launching point
   - Zombie issues
   - Fixed a bug to do with deleting an object while having the context menu open
   - Fixed an activation propagation problem
### Removed
   - UI scale setting (it now resets to 100%)

## [1.2.5] - October 27 2019
### Added
   - Glock 17
   - Desert Eagle
   - PPSH
   - M1 Garand
   - Vector
   - Stielhandgranate
   - Disassembler gun
   - Decimator
   - Total limb crushing (toggleable in settings)
   - Physics iterations slider in the settings menu. Higher values for a more accurate simulation. Lower values for a better framerate.
   - Adrenaline
      - Humans will get a slight increase in strength and consciousness in response to intense pain
   - Changed default jukebox texture
   - Added a new texture to the jukebox
   - Added jukebox context menu options
### Changed
   - Updated sniper rifle sound
   - Improved bruise look
   - Smoothed out the slanted map
   - Crystal sprite
   - Scherbenwerfer sprite
   - You can now hold wrenches
   - Humans bleed out 1.5x as fast
   - Humans and androids can now hold objects with both hands
   - Objects held by humans and androids will now drop on death (of the arm)
      - This also means objects will immediately be dropped when you attempt to pick something up with an incapable arm
   - Firearm performance improvements
   - Increased head joint strength
   - A little extra logging info
### Fixed
   - Fixed the slanted map devouring sharp objects
   - Animation override is now correctly preserved when saving/loading
   - Zombies will no longer remain cowered forever
   - Fixed minor ragdoll problems
   - Fixed incorrect jukebox thumbnail

## [1.2.4] - October 11 2019
### Added
   - Pumpkin
   - Scherbenwerfer
   - Electricity Transformer
   - Mirror
   - The ability to toggle weightlessness on objects
### Changed
- Freezing outlines now disappear after a second
- Crossbow finally has knockback
- Bleeding wounds now heal automatically
   - This also means the lethality of wounds is now based on how deep it is. Syringe wounds heal quicky, while a spear through the stomach won't heal at all.
- Sharp objects can now penetrate multiple objects 
   - **This breaks any lodged objects in saves from older versions**
 - Improved performance of particles
 - Updated to Unity 2019.2.8f1
 - Made androids a bit less powerful (their strength was ungodly)
 - Syringes are now grippable
### Fixed
 - Fixed upper arms locking after life syringe
 - Fixed human heads being ever so slightly offset
 - Fixed decals occasionally rendering on top when they shouldn't
 - Fixed cables should be more stable now
 - Floodlight-light appearing incorrectly underwater
 - Fixed a bug where sharp objects would get stuck in other objects
 - Truck thumbnail
 - A few items refused to interact with water (thank you, hugopolis)
 - Non-existent objects can no longer be undone after clearing the room
 - You can no longer get semi-stuck in the wall when moving the camera using the keyboard
 - Set contraption name character limit to 64
 - Sharp object phasing through universe
   - Hard to reproduce, I think it's fixed now (again)
 - Minor bugfixes

## [1.2.3] - September 29 2019

### Added
- AK-47
- Bus
- Bus chair
- Laser pointer
- Knockout syringe
- Metronome
   - This item is basically a clock. It sends an activation signal every second (unless modified)
- An industrial size piston
- The lightning tool will now charge anything even when no lightning bolt is fired
- Sit pose
### Changed
- The truck's container is now fully transparent
- Simplified animation names
- Worm Staff worms are a little more floppy
- Piston heads are no longer conductive
- Television is heavier
- Thinner fixed cables
- The android no longer appears before the human in the menu
- Increased clarity of tool tooltips
- Text renders a little better now
- Lowered water flaying intensity
- Humans are a little more durable, but they are also more susceptible to falling unconscious
- Androids are no longer as weak
- Androids spark underwater
- Androids no longer make organic noises when their bones break or when their limbs detach
- The lightning tool should be easier to use
- Changed television noise to an actual test card
- Increased drown death time from 2m to 4m
- Drastically improved performance of wires and cables
- Certain context menu options are now hidden unless useful
- Darkened toybox panel
### Fixed
- Frozen ragdolls will no longer attempt to stay upright
- Wrenches will now repair androids more effectively
- Sometimes, humans would be considered alive even when they are obviously not
   - Alive status is now based on the condition of the _Head_ limb.
- Limbs will now lose blood when the skin is burnt off
- Androids are no longer immune to blood decals
- Clamped muscle strength
- Fixed human head texture having a thin white line appearing sometimes
- A lightning bolt will no longer remain on screen after switching between tools during use
- _Rebind keys_ button is a bit larger and darker to make it stand out
### Removed
- Sentry Turret no longer emits electricity upon targeting
- Deafening audio volumes
   - There is a setting to turn it back on if you enjoyed it as much as I did

## [1.2.2.2] - September 23 2019

### Patch notes
Last update had a few issues following the rewrite, this is a quick patch.

 - Humans are now more sensitive to impact damage
 - Limbs now no longer function when their skin is damaged enough
 - Androids don't drown anymore
 - Severe head wounds are no longer survivable
 - Humans have their randomised sizes back
 - Humans once again panic when drowning
 - Arms are no longer super strong so you can move them manually again
 - Fixed sharp items phasing through the universe after stabbing humans
    - If you still encounter this bug, please report it to me.
 - Fixed bug where joint limits would be always enabled when flipped
 - Humanoids no longer have a 0.1% chance of fainting when bleeding
 - Humanoids now take twice as long to bleed out
 - Humans slowly drop to the floor in case of intense blood loss instead of just dying abruptly
 - Acid hurts again
 - Fixed bug where humanoids would stumble backward indefinitely
 - Fixed bone breaking sound being repeated a little too often
 - Lowered cooldown time for the lightning tool from 500ms to 100ms
    - Changed the cooldown time to be independent of slow motion
 - Fixed humanoids hovering after pasting/loading them in
 - Fixed other minor bugs

## [1.2.2] - September 22 2019

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
