# Changelog

# [1.26.1] - god knows

## Changed
 - Explosive barrels will no longer ignite obstructed objects

## Fixed
 - Layering issues regarding objects with multiple sprites (lagboxes, ion cannons, etc.)
 - Syringes behaving incorrectly if pasted/loaded while lodged into a liquid container
 - Attachment point blob in detail mode being visible at the wrong time

# [1.26] - December 29 2022

## Added
 - Wooden Binding
 - Jet Engine
 - Freezing limbs will now damage tissue
 - Metal scraping sparks
 - Activator Electrode
 - You can now edit object rendering layers (context menu option & optional keybinds)
 - Local fire propagation on large flammable objects
 - Procedural gore fragments on crush (disabled by default, enable in settings)
 - Functional weapon attachments (capacitor, explosive, scope, laser, flashlight)
 - Tyres can pop/deflate
 - Burnt leaves will now slowly disappear
 - Brain damage can be disabled in settings
 - "Toggle UI visibility" optional keybind
 - ModAPI.SerialiseJSON, ModAPI.DeserialiseJSON, ModAPI.DeleteJSON
 - Nitroglycerine will explode when the container is charged by something like a battery
 - The optional OnUnload static method is now called when the application is closed for all loaded mods.
 - Bullets can now dismember limbs in addition to them already crushing limbs
 - Fire Extinguisher is a little more animated
 - ModAPI.RegisterCategory
 - Catalog now supports custom categories
 - ModAPI.OnWireDestroyed, ModAPI.OnPinDestroyed, ModAPI.OnLinkDestroyed
 - BallisticsEmitter.OnTracerCreation<LineRenderer> is a UnityEvent that can be used to customise a tracer round when it is created

## Changed
 - Minor changes to ragdoll animation system. Some animations had way too much force behind them and it's now possible for animations to specify a force multiplier.
 - Bullet damage is now based on speed alongside distance and cartridge damage
 - Servos no longer speed up when powered, they only become more powerful. Speed can be changed in the context menu.
 - Life syringe stops seizures
 - Drastically lowered chance of brain damage, it should be a rare occurrence
 - Lowered chance of concrete rebar appearing in concrete debris. It's completely disabled when Fancy Effects is disabled.
 - Slightly improved tesla coil arcs
 - Increased water impact damage 
 - Bullet casings now shrink when despawning
 - Deflated tyres slightly deform when in contact with an object
 - Oxygen deficiency may cause brain damage
 - Low blood pressure may cause brain damage
 - Lowered brain damage posturing time
 - Increased crush-by-gunshot chances a bit
 - Seizures can stop the heart
 - Slightly lowered entity impact damage
 - Bleeding particles collide with the world when Fancy Effects is enabled
 - Fire Extinguisher is a little heavier now
 - Increased thermal pulse intensity from nuclear explosions
 - Increased drag underwater
 - Made androids less vulnerable to explosives
 - Made many changes to the body heat system and responses to environment temperature. Humans are more resistant to cold environments. They won't freeze as quickly and will often pass out before dying if their body temperature is too low.
 - Changed sharpness velocity threshold calculation. Lower softness values are now more effective
 - Improved wood impact VFX
 - Improved thruster SFX
 - Improved propeller SFX
 - Improved ricochet SFX variety
 - Improved fire extinguisher particles
 - Lowered audio range of mini thruster
 - Improved pumpkin destruction effect
 - Decreased cannon shockwave
 - Falling embers now collide
 - Made acid less effective on androids
 - Laser colours can be much darker
 - Explosions can now completely crush bodyparts if "procedural fragments" is enabled
 - Increased G1 SMG, SMG, and Minigun spread
 - Increased LMG heat up speed and added a little glowy bit at the end (will automatically be removed when overridden with a mod. Use ModAPI.KeepExtraObjects())

## Fixed
 - Older contraptions having firearms with incorrect reflection sounds
 - Stupid memory leak to do with custom human textures
 - Ray cannon going insane on void & other maps occasionally
 - Fragility slider not showing enough digits
 - Crossbow bolts spinning forever
 - Some energy sword problems
 - Item persistence bugs (normal sized bug) (you may have to do the achievement again)
 - Tree collision
 - Human feet are no longer unnaturally resistant to being crushed
 - Phase link slightly affecting center of mass
 - Phase link being deletable without being visible
 - Minor performance improvements to do with phase links and other tools
 - Some deletion stuff
 - Flamethrower wouldn't burn stuff up close sometimes
 - Pin hover stuff
 - The game will now delete older logs as to keep a maximum of 25 logs in the log directory
 - Menu escape issue
 - Bug where limbs would cool down when dead despite blood flowing through them
 - Bug where cardiopulmonary bypass machine continues to provide oxygen even when turned off/broken
 - Electricity particles not scaling with the object
 - Some major liquid system problems
 - Automatic firearms shooting two bullets as their first shot sometimes
 - Weird deletion message stuff
 - Things can no longer breathe when submerged in ice
 - Humans unable to grab things after copy/pasting
 - Other minor bugs

## Removed
 - Android instant death on dismemberment

## Additionally
- Many changes and improvements to the modding wiki.
- Aspa102
- [You should read our weekly blog for updates on all our projects](https://www.studiominus.nl/blog/)
- I need to remind myself to **never** make updates large and infrequent. It's a lot better for everyone involved to make them frequent and smaller. Ideally focused on a theme or single feature implementation. This shouldn't happen anymore from now on.


# [1.25.4] - July 15 🎈 2022

## Fixed
 - Mods failing to compile occasionally on start
## Removed
 - You know what

# [1.25.3] - July 15 🎈 2022

## Changed
 - Made seizures a little less intense and lowered maximum duration from 5 minutes to 30 seconds
 - Pain animation is less strong, again
 - Painkiller can now help with seizures

# [1.25.2] - July 14 2022

## Added
 - Seizures

## Changed
 - Made tritium more likely to heal brain damage
 - Brain damage is less likely to occur
 - Brain damage postures are no longer permanent, but the being will be noticeably incapable and might occasionally collapse or have a seizure

## Fixed
 - Brain damaged people still walking and stuff if instructed to
 - Some gorse gore effects having incorrect colours
 - Gorse ball impact vfx being wrong
 - Cobblestone wall debris going insane in water

# [1.25.1] - July 13 2022

## Fixed
 - Gorses and androids not working at all

# [1.25] - July 13 2022

## Added
 - Split up settings into more categories: 
    - General
    - Gore
    - Visual effects
    - User Interface
    - Video
    - Audio
 - Goreless mode: no blood, no gore
 - Brain damage and relevant poses. Permanent unless treated.
 - Entity fragility multiplier in Gore settings. Make humans (etc.) more or less fragile as you play.
 - Dismemberment could now expose stringy tissue that will loosely hold the limbs together
 - Limbs with enough flesh on them may eject chunky particles when shot, similar to brain-matter particles
 - Cobblestone wall
 - Stone brick wall
 - Stone brick
 - Ray Cannon
 - Liquid Duplicator
 - Cardiopulmonary Bypass Machine
 - Minor extra details to the default bullet impact effect (only visible when Fancy Effects is enabled)
 - Foliage leaves sway ever so slightly 
 - Dimly lit objects are now desaturated to prevent unnatural looking brightness from vibrant objects
 - Burned foliage will now shimmer and char
 - Destroyed concrete now has loose, sharp rebar 
 - Some more bullet ricochet sound variants
 - Some particles to limb crushing effects
 - Discord server invite link to Information menu

## Changed
 - Beam rifle beam will now crush limbs if they can't be sliced off
 - Brain matter particles are sometimes red
 - Detaching the head from the torso will instantly kill the organism
 - Flamethrower will heat things up less quickly
 - Worm staff wounds now are counted as stab wounds in the entity inspector
 - Decreased bleeding rate when most skin is gone
 - Energy Sword no longer sets everything on fire instantly
 - Doubled activation propagation limit
 - Firearm casings that are ejected now scale with the weapon
 - Blaster weapon muzzle flashes
 - Siren texture
 - Minor changes to fire particles
 - Changed Sentry Turret gun sound
 - Sentry Turret now targets torso over anything else
 - Human blood regeneration is slower
 - Achievement icons updated to current sprites
 - Made the plate stronger
 - Tritium can heal a dead brain
 - Blood no longer regenerates if the limb is bleeding or dismembered
 - Bandages' redness is now based on bleeding intensity 
 - Impact damage on organisms is now much more dangerous. It can propagate through from the impact limb to other connected limbs to roughly approximate what would happen in real life.

## Fixed
 - Auto healing again
 - Immortality serum
 - Acid is more effective and consistent
 - Burn wounds regenerating despite "auto heal injuries" being off
 - Heart rate monitor inaccuracy
 - Saving broken pistons being all messed up
 - Disassembler still discharging despite being broken
 - Firearms not always passing in the Cartridge
 - Slider slider width not adjusting to the actual scale
 - Impact intensity averaging calculation now removes outliers
 - Sentry turret no longer targets dead limbs if the human is still alive
 - Beam rifle beam is no longer effectively infinitely thin 
 - Flamethrower going through walls occasionally
 - Flamethrower going through very small gaps
 - Fire extinguisher and flamethrower particles scale with the object
 - Critical drag tool bug
 - Tempered glass
 - Syringes and other small sharp things getting stuck inside people and potentially breaking their bones
 - Energy Sword impact vfx position
 - Weird debris issues to do with undoing
 - Minor performance improvements
 - Decimator will no longer occasionally be extremely loud when deleting multi-part objects

## Removed
 - "You can set your collision mode to "Discrete" for a significant performance boost!"

# [1.24.6] - May 26 2022

## Changed
 - Immortality serum now heals skin damage too
 - Minor tweaks to body shader

## Fixed
 - Healing dismemberment wounds being abrupt
 - Laser receivers still sending signals even when broken
 - Key triggers still sending signals even when broken
 - Resizing objects that have been disintegrated
 - Defibrillator reliability issues

# [1.24.5] - May 24 2022

## Added
 - Cyrillic support

## Fixed
 - Logging oversight

# [1.24.4] - May 24 2022

## Changed
 - Hover thruster max height is now 10 km

## Fixed
 - Brain-death being way too hard to heal
 - Androids being impossible to revive sometimes
 - Liquid exit tolerance & reliability
 - Tritium permanence 
 - Auto-healing

# [1.24.3] - May 23 2022

## Added 
 - Burn damage can heal
 - Adrenaline undoes numbness

## Changed
 - Bullet-holes can be a bit smaller

## Fixed
 - Even more burning issues (endless burning)
 - Regeneration speed being way too slow
 - Brain-dead state not working correctly
 - Tempered glass undo not working 

# [1.24.2] - May 22 2022

## Fixed
 - Burning issues
 - Inspector issues 
 - Other issues that are too small and numerous to list

# [1.24.1] - May 22 2022

A small patch to fix issues people have encountered & bonus additions.

## Added
 - "Heart stopped" in living entity inspector if the heart has stopped working
 - "Brain-dead" in living entity inspector if... yeah

## Fixed
 - Human water impact damage is no longer excessive
 - Error in bullet damage-by-distance-calculation
 - Bullet-wound damage response curve. The contrast between small round damage & big round damage is greater and more noticeable. 
 - More electrocution issues
 - Android durability being almost infinite

# [1.24] - May 21 2022

## Added
 - Liquid canister. This is a high capacity container that is vulnerable to bullets and has a variable buoyancy.
 - Painkiller syringe
 - Humans will pass out when they experience too much g-force
 - Boat motor reverses on red signal
 - For modders: support for transparent liquids 
 - For modders: Liquid.GetDisplayName()
 - For modders: BloodContainer.ForceCalculateComputedColor

## Changed
 - Completely rewrote body shader (this may make humans from older contraptions look weird)
   - Blunt damage causes bruising (new look)
   - Bullets make bullet holes
   - Stabbing makes stab wounds
   - Touching hot objects & friction causes burn wounds
   - You can switch back to the legacy shaders in the general settings menu
   - **Important for modders**: wound intensity is now inverted (normal). The higher the Z component, the more intense the wound.
 - Bullet impacts on bodies of water are more intense
 - Stopping time has a shorter transition
 - Androids are more durable
 - Minor rendering optimisations
 - Other minor optimisations
 - Changed bullet hardness & damage distance calculations
 - Limbs don't drain their liquid as fast when bone is exposed
 - Humans don't panic as easily when shot
 - Humans wince more when shot
 - Humans and gorses regenerate blood slowly, if they're alive
 - Bullets have 50% more impact force
 - Tritium glows when seen in transparent containers
 - Made punctured lungs more dangerous
 - Increased g-force resilience
 - Decreased human drown time
 - Boiling bodies of water have no buoyancy 
 - Changing weather settings like rain, snow, and fog will now happen smoothly instead of abruptly.
 - G-force damage no longer occurs when the organism was frozen
 - Improved distant large explosion sound
 - Changed AK-47 sfx
 - Changed AR sfx
 - Changed Submachine gun sfx
 - Changed Shotgun sfx
 - Changed Sniper sfx
 - Swapped old Rifle sfx for sniper SFX 
 - Improved Gorse collision
 - Increased explosion shrapnel lethality
 - Made Ultra Strength Serum more potent
 - Decreased bleeding particles intensity
 - Minor tweaks to entity body temperature maths
 - Increased body bullet impact sound volume
 - Gave liquids nicer names
 - Made human pain animation a little less rigid
 - Organisms rot slower
 - Increased minimum impact damage threshold for limbs
 - Heat capacity is now calculated using object mass in addition to size & material properties
 - Lowered object to air heat dissipation 

## Fixed
 - Android circuit layer transparency 
 - Improved limb liquid circulation
 - Fireworks detail view radius visible for too long
 - Concrete debris suddenly disappearing
 - Made rescaled living entities a little more stable. 
 - Boat motor saving issues
 - Slider disintegration issues
 - Unnecessary memory usage
 - Electrocution issues
 - Workshop upload dialog box being weirdly sized
 - Fluorescent bulb glow overlay appearing in front of everything
 - Issues :(
 - Detectors emitting signals even when broken
 - Human flesh layer not covering all bones

## Removed 
 - Removed coagulation concentration calculation

# [1.23.10] - April 15 2022

## Fixed
 - Now it has to be impossible for the compiler server to stay alive please god

# [1.23.9] - April 14 2022

## Fixed
 - Centrifuge bug on low settings
 - "Sharing violation" error while compiling mods

# [1.23.8] - April 12 2022

## Changed
 - Should be impossible for the compiler server to stay alive

# [1.23.7] - April 11 2022

## Note for Windows 7 users

Your operating system is obsolete. But if you want to keep using it anyway, you will probably need a little update:

[KB3063858 for 64 bit (probably what you need)](https://www.microsoft.com/en-us/download/details.aspx?id=47442)

[KB3063858 for 32 bit (if your computer is older than you)](https://www.microsoft.com/en-us/download/details.aspx?id=47409)

## Added
 - Faster mod loading / compilation
 - Small Boulder
 - Fluorescent Lamp
 - Invisible particle projectors are now visible in detail view

## Changed
 - Instant death poison is instant again
 - Made bottle stronger
 - Boat motor no longer electrocutes everything when charged
 - Boat motor now breaks at 800 degrees Celsius
 - Organism inspector now considers an organism with a dysfunctional brain to be fully dead.
 - Minor changes to blood pressure calculation
 - Detached limbs no longer have a heartbeat lmao
 - Spotlights emit some softer light too
 - Mod compiling is now more compatible with older systems

## Fixed
 - Decal layer stuff
 - Android arm layer stuff
 - Substructure lift layer stuff
 - Minor optimisations
 - Physics audio volume inconsistencies
 - Minor change to a bus texture 🟥
 - Emergency stop button on lift not working sometimes
 - Celsius*

# [1.23.6] - April 3 2022

## Added 
 - "Dynamic" collision mode. Dynamic mode switches between discrete and continuous based on velocity. It serves as a middle-ground between the two, being more reliable than discrete mode but not as CPU-hungry as continuous mode.
 - Android "skin" can be burnt off, just like pre-temperature-update versions
 - Boat motor

## Changed
 - Minor optimisations to do with dragging
 - Slowed human internal temperature transfer rate
 - If the heart is stopped or blood flow is blocked, organisms no longer lose all blood pressure immediately
 - Made organisms more vulnerable to hot/cold environments
 - Minor changes to metal impact VFX
 - Save files containing foliage are now much smaller and will take less time to load/save
 - Leaves will resize with the rest of the foliage 
 - Ceiling turret is no longer invulnerable to heat 

## Fixed
 - Weapons (and other things) not saving their position properly when held by a ragdoll
 - Some spelling inconsistencies
 - Black hole not doing the black hole thing sometimes
 - Modded liquids will now correctly cause a contraption to require mods
 - A bug, believe it or not
 - Crate debris fuckery
 - Bug to do with piston correction
 - Winch connector thing being weird when flipped
 - Android arm decal rendering
 - Moving foliage around in pause mode will now bring leaves with them
 - Problem to do with car doors being broken and then being copy-pasted

## [1.23.5] - April 1 2022

## Changed
 - Water breathing serum now lasts forever

## Fixed
 - Water breathing syringe bug
 - Logging issue

## [1.23.4] - March 30 2022

## Changed
 - Made the ambience in the Small map a lot less loud
 - Minor performance improvements

## Fixed
 - Potentially unachievable achievement

## [1.23.3] - March 28 2022

## Fixed
 - Liquid mixing problems again

## [1.23.2] - March 28 2022

## Fixed
 - Liquid mixing problems

## [1.23.1] - March 28 2022

## Fixed
 - Wheel problem
 - Button problem

## [1.23] - March 28 2022

## Added
 - Substructure map
 - Mechanical Belt
 - Resizable Housing (colourable box that maintains a correct texture when resized)
 - Bottle
 - Power Hammer
 - Trees
 - Bushes
 - Magnum Revolver
 - Bazooka
 - Liquid centrifuge
 - Spot light
 - Normal wheel
 - Particle Projector
 - Key triggers now clearly show what key they're assigned to in Detail View. They can also be given a description.
 - Contraptions now have an "info" button. It'll show you required mods and some other useful information.
 - Some more bone breaking sounds
 - "Slowly heal injuries" is now togglable 
 - "Open in Workshop" button, if applicable
 - Thumbnail size warning on Workshop upload
 - "Ambience Highpass" setting. It allows the player to set a highpass cutoff frequency for the ambient noise. **This is useful if you suffer from crackling audio issues.**
 - Search bar in mod menu
 - Better explosion shrapnel. Some explosions will now emit shrapnel (invisible, behave identical to bullets)
 - More wooden strut stress sfx
 - Optional "Choose object under cursor" keybind. It's like Minecraft middle click.
 - Made soap work just by sliding too
 - Fire embers (only visible when Fancy Effects is enabled)
 - Laser pointer colour can be changed
 - Organisms have a chance to walk a bit when shot
 - When shot in the head, there is a chance for visual brain matter to fly out
 - Distant SFX. Guns and explosives now have special sounds that are heard when they're distant.
 - Clearing everything will now reset the map too
 - Overwriting a contraption that you've uploaded to the Workshop and then uploading it again will update the existing Workshop item.
 - Destructible machinery can now be made indestructible using the context menu
 - Flamethrower flames and fire extinguisher... puffs (??) now collide with objects, they have no effect on things behind walls
 - Contraptions that depend on mods will now have a list of required mods added to the description. **There is no way for me to automatically add required items to the Steam upload. You need to do this yourself.**
 - For modders: LiquidMixingController. [Visit the modding wiki for more information.](https://www.studiominus.nl/ppg-modding/tutorials/tutorialMixing.html)
 - For modders: the SkipSerialisationAttribute can now be applied to a class as well. This will exclude the entire component from the serialisation process.
 - For modders: A Map object now has InstantiateOverride. This is an Action that, if not null, will be called on map load instead of instantiating the Prefab. The proper container is provided as a parameter.

## Changed
 - "Biohazard" category is now "Chemistry" (FindCategory treats them as the same)
 - Made metronome more consistent
 - Renamed "Wheel" to "Wooden Wheel"
 - Minor changes to metal hit effect
 - The exact colour of the LED Bulb can now be set (this replaces all other LED Bulbs)
 - Broken electronics spark SFX
 - Pistons will keep pushing/pulling. They can no longer be forcibly moved by other objects without them returning to their target state.
 - The Tank is no longer a solid block of metal. It has an engine and gas tank, just like the car, and its turret base is detachable.
 - Made humans heavier and stronger
 - Blood will no longer spill out when a limb is stabbed. Instead, most of the blood will stay inside until the sharp object is removed.
 - Reordered some buttons on the contraption button in the toybox
 - Made the nitro-glycerine explosion more powerful again
 - Minor changes to minigun behaviour
 - Made bell a bit less loud
 - Changed minigun SFX
 - Minor change to rocket launcher SFX
 - Small change to sniper rifle SFX
 - Changed 120mm cannon SFX
 - Changed tank cannon SFX
 - Increased tank barrel weight
 - Increased tank cannon recoil
 - Decreased tank suspension strength
 - Decreased tank speed
 - Tank muzzle blast is a little more dangerous and is much larger
 - Decreased ambient sound rate on Humongous
 - Decreased bullet drop
 - Phase link is now only visible in detail view
 - Increased default mod compilation duration limit and increased maximum loading time from 60 seconds to 120 seconds
 - Selection outline is a little less vibrant
 - Minor changes to human bruise colour
 - Minor changes to human blood impact
 - Increased grenade fuse from 2 seconds to 4 seconds
 - Mods that use the "Application" identifier are marked as suspicious
 - Rockets launched from the standard rocket launcher will slow down more underwater and will get stuck inside immobility fields
 - Decreased activation signal amount warning sound rate
 - Increased activation signal limit
 - Layering changes to the tank
 - Lowered impact force of bullets on very hard objects (like bulletproof plates)
 - Minor changes to brick impact VFX
 - Decal sorting order stuff
 - Made that little orange thing in the corner of outdated contraptions a bit smaller
 - Small wood impact is a little louder
 - Made sliding sound less loud
 - For modders: deprecated Hover.collider and all wire colliders
 - Removed very low frequencies from ambient hum
 - Pistons now stop working completely when broken
 - Made some bullet impact SFX a little less loud
 - Increased "stop animation on damage" damage threshold

## Fixed
 - Absolutely terrible oversight in the serialisation and deserialisation of wires. Wires should no longer turn pink / disappear after paste or load. This should also fix a whole bunch of other problems to do with the serialisation of specific objects.
 - An awful design flaw to do with continuous activation signals. This should not introduce any unexpected behaviour unless you expect something to be broken. Some contraptions may rely on this inconsistency, and they will break. Most contraptions will benefit from this and behave a lot more consistently. It should also reduce (pretty much eliminate) activation signal limit warnings. 
 - Improved fast moving wire performance
 - Debug messages doing the DRAG SELECTED thing.
 - Glass no longer increases detector range if placed in front of a mirror
 - Zombies moving even though they're dead (more deader)
 - Other minor performance improvements
 - Fixed an LED bulb issue that you never noticed 
 - RemoveLiquid bug that can cause liquid underflow
 - Some pumpkin stuff
 - Weird explosion miscalculation (`CreatePulseExplosion`)
 - Minor firearm bugs
 - Liquidentifier going nuts in lava
 - Bicycle is now made of metal too, just like the others
 - Bug where explosives could trigger other explosives infinite times
 - Some deletion stuff
 - Soap problems
 - Water making the entire map float
 - Outlet liquid decal issues
 - Contraption synchronisation can time-out (20 seconds per item, just to prevent an infinite loop in case Steam loses its mind)
 - Toybox scrollbar stuff

## Removed
 - Removed liquid pressuriser sound
 - Removed rotor sound
 - Expanded gore is gone

## [1.22.3] - 2 December 2021

## Added
- Accelerator energy weapon
- Archelix Caster energy weapon
- Plastic explosive
- Liquid.GetAll()
- The inspection display now shows if the entity has punctured lungs
- Punctured lungs cause pain
- SimpleLightingEmitterBehaviour.Instance.Emit
- A few new minor Steam achievements
- A warning that appears whenever the maximum activation signal limit is reached
- You can press escape to stop resizing

## Changed
- Lowered likelihood of punctured lungs
- Minor change to sniper rifle SFX
- Bullet wounds can fully heal if properly treated
- Internal bleeding will heal faster
- Gave the immobility field a little more health
- Decreased required temperature for organisms to start shivering
- Liquid effect intensity is now often based on the concentration of the liquid inside the container

## Fixed
- Incorrect ceiling turret aiming
- Minor memory leaks (minor as in "minor catastrophe")
- Minor performance improvements
- Flamethrower issues
- Key rebinding issue when trying to bind to "escape"
- Strange problems setting the contents of multiple text displays/radios/hologram displays at once
- "Previous texture" not always working
- DRAG SELECTED
- DRAG SELECTED
- DRAG SELECTED

## [1.22.2] - November 10 2021

## Fixed
- Fixed some out-of-bounds stuff again
- Made PhysicalBehaviour.IsUnderwater's set accessor public again

## [1.22.1] - November 9 2021

## Added
 - Mods now show if they have timed out

## Changed
 - Decreased likelihood of internal bleeding
 - Reconstructor will help heal internal bleeding
 - Sentry turret is now a little more vulnerable
 - Fireworks can explode when shot

## Fixed
 - Infrared thermometer incorrect limits
 - Gate double trigger not existing
 - Sentry turret debris issues
 - Bicycle disintegration bug
 - "Bleeding" showing up in inspection display despite lack of visual bleeding

## [1.22] - November 1 2021

## Added
 - Much better bells. You can select a piano key in the context menu.
 - Infrared thermometer
 - Liquid outlet
 - Thermal vision
 - Vases
 - Wire direction snapping
 - Detached 30mm HEAT autocannon
 - Entities feel momentary pain when stunned
 - "Stop animation on damage" setting
 - "Set object temperature" context menu option
 - Escape key escaping things
 - Objects are now destroyed if they are out of bounds for over 5 seconds
 - "Recompile" button that is shown when a mod failed to compile. This way you don't need to restart the entire game when you are developing a mod.
 - Maximum mod compilation duration setting. 10 seconds by default. A mod is only allowed to take this amount of time for compiling, otherwise its terminated and ignored.
 - Blood decal & particle colours are now accurate to the actual liquid inside the body
 - Water cleans objects
 - Balloons now pop under pressure
 - Exit wounds for stabbing 
 - Humans can get paralysed if their spine breaks
 - There is a chance that an injury punctures the lungs of a human, which can cause low oxygen levels and death
 - Organisms now have specific "vital" spots inside their body. For example, head injuries are no longer necessarily a brain injury.
 - Organisms can now bleed internally. Internal bleeding can cause many issues, most obviously twitching, slowness, and loss of balance (in case of a head injury). Major internal bleeding results in death.
 - More intense bullet metal impact sounds
 - If set to "Drain", the blood tank can now spill into other containers. This means you can finally make a nitro-glycerine shower. It can also spill onto non-container objects, but this **will not** transfer the liquid effects onto that surface.
 - Firearms can accidentally discharge when dropped
 - Multiselect using shift (by default)
 - Toybox size is now remembered
 - A few optional keybinds
 - Unbind button in keybind menu

## Changed
 - Humans regenerate limb integrity slowly
 - Lowered contraption spawn outline delay
 - Living tissue regenerates visual blunt damage slowly
 - Adjusted impact damage so that head injuries are more dangerous
 - Fire kills less quickly
 - Increased general impact damage severity
 - Decreased blood impact particle intensity
 - Decreased bleeding particle intensity
 - Other minor changes to humans
 - Disassembler is more likely to disintegrate things
 - Increased maximum bullet penetration iterations to 128. This will make thick, soft obstacles more penetrable.
 - Some firearm SFX changes
 - Wood impact SFX
 - Increased blood vessel wire transfer speed
 - Minor changes to liquid rules
 - Minor changes to the machine gun and 30mm cartridge
 - Joint stress sound rate
 - Beam rifle now heats up objects it strikes
 - Lightbulb flickers a bit
 - Blaster bolts heat up objects that they reflect off of
 - Increased rocket launcher impact dismemberment chance
 - Multithreaded the ambient temperature system
 - The ambient temperature grid can now propagate more effectively
 - Replaced "Symphony No.40, Mozart" with "Danse Macabre, Saint Saëns 🎃" in the Jukebox.
 - Minor changes to keybind page
 - "Show selection/freezing outlines" settings is now called "Show hovering highlights". It will also disable the red wire highlights.

## Fixed
 - Minor optimisation
 - Minor bug fixes
 - Weird bandage tool bug where you could attach it to other wires
 - Water splashing being audible from seven light years away
 - Ceiling turret not correctly saving/loading frozen state
 - Syringes not being affected by pressure system
 - Accidental overwriting of contraptions
 - Bug where you could resize the toybox with middle mouse button
 - Occasional flashes of light when spawning in items
 - Bug causing knockout poison to appear pitch black
 - Center of mass being all messed up when the object is resized or flipped
 - Pull/push powers occasionally causing teleportation
 - Disappearing center of mass etc.
 - Accumulator not having a heat shield option
 - Object pooling issue
 - Lingering limb status UI things after deserialisation
 - Conveyor belt pinning serialisation issues
 - Lingering objects after disintegration

## Removed
 - The old bells. Contraptions with old bells in them will still work.
 - PersonBehaviour.AverageAngle
 - "Liquid overflow limb exploding" setting

## [1.21.3] - August 23 2021

## Added
 - Cable. An indestructible non-conductive wire.

## Changed
 - Renamed a few items
 - Made destructible propagation wires less fragile
 - Slightly faster contraption spawning / pasting
 - Shards and crossbow bolts fired from their respective launchers no longer collide with each other
 - Explosives heat up objects less intensely

## Fixed
 - Steam warning appearing too often
 - Out of bounds hover height for hover thrusters
 - The game now falls back to the object center when calculating the center of mass for frozen objects
 - Crate debris not being removed correctly
 - More consistent contraption mod detection
 - Propagation wire destructibility issues (is that a word?)
 - Activation transformer only outputting a green signal
 - Minor bug fixes
 - Center of mass gizmo being all jittery
 - Frozen organisms not experiencing some things
 - Tool shortcut subtool order

## [1.21.2] - August 19 2021

## Added
 - Hover thrusters can now change height using signals. Red increases hover height by 10 cm every use (or 5 meters per second when used continuously), blue decreases by the same amount.

## Changed
 - Falling animation
 - Dismemberment is now painful
 - LED Bulbs can now break
 - G1 SMG sounds

## Fixed
 - Humans no longer die immediately if their arms are ripped off
 - Older outlines being all warped
 - Some effects not being removed when "Clear everything" is pressed
 - Laser not scaling correctly

## [1.21.1] - August 18 2021

## Changed
 - Hover thrusters now have an editable hover height (context menu). Energy only makes it more powerful.
 - Water splashes are no longer created if the object is moving too slowly

## Fixed
 - The camera going insane when following disintegrated things
 - Underwater sound starting too early
 - Memory leak
 - Much faster map switching and contraption saving
 - Activation toggle still working when broken
 - Resize action in context menu not closing the menu
 - Other small bugs
 - Outline (de)serialisation issues


## [1.21] - August 17 2021

## Added
 - Liquid pressuriser
 - Liquid pressure valve
 - Destructible activation propagation wires
 - Hover thruster
 - Activation toggle
 - Accumulator battery
 - Automatic spike gun
 - You can now change the range of a detector using the context menu
 - Red LED, Blue LED, Green LED, White LED
 - More mystery liquids
 - Lava pools now work nicely with ambient temperature
 - All contraptions saved from now on will include a list of required mods. When selecting a modded contraption, the game will display a list of required mods if you don't have them installed or enabled.
 - Scrollbar to the mod menu and toybox
 - More ambient sounds
 - Gate now has a double trigger mode
 - Some UI sounds
 - A clear "Steam uninitialised" warning dialog box

## Changed
 - Simplified some object colliders
 - Bone breaking sounds
 - Minor texture changes
 - Missile launcher missile is now disarmed until its fins are deployed
 - Made the phase link smaller
 - Ceiling turret moves less smoothly and more robotically
 - Laser performance improvements
 - Detector performance improvements
 - Detector rays are a little brighter
 - Dialog boxes are clearer now
 - Other major performance improvements
 - Hovercars now hover over water
 - Increased mouse scrolling speed in menus
 - Some UI sounds
 - Bone breaking poison is less instant
 - Decreased the chance for damage to the upper body to do damage to the heart
 - Changes to the internal map system. Note to custom map creators and users: your maps will inevitably break in the upcoming updates. They may work to an extent but you should consider them obsolete.

## Fixed
 - A broken plate being heavier than a normal one
 - Display text change dialog not being pre-filled with the current text being displayed
 - Stuff being rendered outside of map bounds
 - Some items going haywire inside lava
 - Context menu closing when the scroll wheel is clicked
 - Valves still transferring pressure when closed
 - Channel-related bug with the gate
 - Liquid related bugs
 - Detectors, lasers, and the missile launcher detecting themselves when moving fast
 - Lasers blocking their own beam
 - Minor disintegration & crushing bugs and also performance improvements
 - Item persistence bug
 - A memory leak
 - Metal detector not considering some items metal
 - Small buttons going haywire in water and lava
 - Heartrate Monitor issues
 - UI lock when attempting to publish a contraption to the Workshop before Steam is initialised
 - Debris not being scaled with the destroyed object correctly
 - Camera trying to follow disintegrated/crushed objects
 - Other minor bugs

## [1.20] - July 28 2021

## Added
 - Lava map
 - Lava pool to Hybrid
 - Buttons have a double trigger mode
 - Underwater objects may transfer charge to other near underwater objects
 - Tempered glass pane
 - You can hold M (can rebind) while using pins to snap to the center of mass of the underlying object. This is useful for things like putting pins in the exact center of wheels. It also magically allows you to put pins outside the object. This may be extended to other tools in the future, but it's just pins for now. It's pins.
 - Liquid container pressure now travels through valves and such. This may introduce some unfamiliar, however correct, behaviour.
 - ModAPI.OnLinkCreated and ModAPI.OnPinCreated events. The modding wiki is being worked on intensely so these events may not be documented for a while. They are invoked when a link device is created (currently only the phase link) and when a pin is created, respectively.
 - Partial proper documentation: https://www.studiominus.nl/ppg-modding/internalReference.html. It isn't completely done yet so there may be some issues. Not everything has an explanation yet but I have done the most important parts.

## Changed
 - Rewrote button behaviour
 - Default value for "Liquid overflow limb exploding" setting is now "Disabled"
 - Made the "Pacifist" achievement less strict.
 - LMG belt is now lighter
 - Minor texture changes
 - Hybrid thumbnail change
 - Extended environmental setting numerical limits. Gravity can now go from -200 to 200. Ambient temperature can now go from -100 to 9000 degrees C

 - ExplosionCreator.CreateExplosionWithWater no longer asks for a water surface level
 
## Fixed
 - Human visual wound serialisation issues
 - Acid inconsistencies
 - Limb crushing inconsistencies
 - Impact intensity inconsistencies
 - Performance improvements
 - Center of mass indicator bugs
 - Resized wings violating the laws of physics
 - Incorrect layering of worm staff worms
 - Syringe and other stabby item problems to do with limb crushing and disintegration
 - Pink enhancing serum can no longer weaken limbs
 - Major water bugs (this changes the WaterBehaviour significantly and if your mod depends on this then it will break)

 ## Removed
 - That "Made it easier to grab moving objects while following them" thing because it actually made things less easy

## [1.19.2] - June 28 2021

## Added
 - Setting to disable liquid-overflow-limb-explosion

## Changed
 - Syringes won't push liquid into a limb if it already has some in it
 
## Fixed
 - Keeping syringes in a human for a prolonged amount of time will no longer destroy them
 - Minor performance improvements & bug fixes

## [1.19.1] - June 27 2021

## Added
 - Limbs explode if pumped too full of liquid
 - Water breathing syringe
 - Fusion bomb
 - Mystery liquids
 - Liquid valve
 - Nuclear weapons may destroy electronics if in line of sight

## Changed
 - Made it easier to grab moving objects while following them
 - Drastically decreased the capacity of the tank in a car
 - Made humans a little stronger
 - Atom bombs glow a bit
 - Beings don't start panicking the moment they're under water
 - Rewrote limb connectedness system. For mods, this means that `CirculationBehaviour.IsConnectedToMainBody` and `CirculationBehaviour.IsDisconnected` are obsolete (still available with behaviour unchanged). Use `Limb.NodeBehaviour.IsConnectedToRoot` instead.
 
## Fixed
 - Camera locking bug when following things
 - Beings being able to live without blood
 - Minor bugs
 - Incorrect temporary body liquid behaviour
 - Weird spawn silhouette delay bug

## Removed

## [1.19] - June 19 2021

## Added
 - Rope
 - Stronger spring variant
 - Empty syringe
 - Ceiling sentry turret
 - Mending syringe
 - Hold the spawn key when spawning contraptions to see their silhouette before placing them down. **This only applies to all contraptions saved in or after this version.** This also applies to copying/pasting using the shortcuts.
 - Empty syringes can push, pull, or be idle. Just like the blood tank.
 - Limbs no longer have an upper bound on their liquid capacity.
 - Liquid identifying machine. It displays the make up of its contents.
 - Blood tank context menu options for each mode
 - Gate "max power" property that you can set using the context menu.
 - Minor details to most maps
 - Brightness setting

## Changed
 - **The entire syringe system. This will destroy all syringe mods created before this version.** All syringe behaviour is now based on liquids. Syringes are liquid containers and every syringe effect is the result of foreign liquid entering the circulation. All syringes, except the empty syringe, are infinite.
 **Attention to modders: you can derive from "OldSyringeBehaviour" instead of "SyringeBehaviour" if you want to keep using the old system.**
 - Almost all spawnable item thumbnails
 - Map ambience is now stereo
 - Bandages will now prioritise connecting to the same object. This makes applying bandage a lot easier.
 - Beings react a little more intensely to being shot
 - Underground tunnel in Hybrid is better lit
 - Syringe appearance
 - Made rope catenaries more accurate
 - Minor performance improvements
 - Made context menu scrolling faster
 - Balloons pop sooner
 - Some electronics are shielded from heat damage on spawn
 - Nitroglycerine is now harmful in large doses

## Fixed
 - Shock detector not sending out a signal to all channels
 - Some platform specific overrides
 - Audio sliders not updating the volume while sliding
 - Gate not having the correct threshold input dialog
 - Odd transmitter sound artifacts & other issues
 - Framerate dependent splash effects
 - Potential audio clamping bug 
 - Major liquid system problems. This _may_ influence older saves with humans in them.
 - Major serialisation issues
 - Blood tank drain particles being the incorrect colour
 - The inspector window "blood amount" value no longer counts other liquid types
 - Shotgun collision boxes
 - Abyss uneven platform height
 - Missing Physics Gun init sound
 - Human reaction to disconnected limbs burning
 - Minor bugs

## Removed
  - Pink Syringe fog particles

## [1.18.1] - May 30 2021

## Added
 - Animations for most traditional firearms
 - Living things now have an internal temperature
 - Internal temperature is shown in the Inspector panel
## Fixed
 - Muzzle flashes not correctly scaling
 - Environment tab not resizing with the containing panel
 - Broken chair being way too rigid
 - Table & chair being too resilient
 - Weird text rendering artifacts (long overdue)
 - Organisms not burning correctly

## [1.18] - May 29 2021

## Added
 - Ion thruster
 - Flintlock pistol
 - Lance
 - Most explosives heat up affected objects
 - Utility workshop tag
 - An alert that tells you which mods are significantly affecting load times
 - Small button to export game debug info
 - The toybox panel is now resizable
 - Wooden furniture is now destructible
## Changed
 - Rewrote most Steam integration, mod loading, and contraption loading to be done in the background. This should fix the phenomenal startup times if you have hundreds of mods. Do note, however, that I can't control what modders make their mods do upon loading. Some mods may still freeze the game and there's nothing I can do to prevent that.
 - This update will forcibly recompile all your installed mods. If you have lots of them, this will take a while. This will only happen once, though.
 - Also switched to Facepunch's C# implementation of Steamworks which you won't really notice.
 - Minor changes to some particle effects
 - Completely changed the settings menu. It is no longer a weird game of Tetris
 - Disallowed mods to use shady code (toggleable in settings)
 - Tank shells are explosive
 - Made humans less resilient to extreme ambient temperatures
 - Lightbulbs are less hot
 - Slight texture changes
 - Energy swords deflect blaster bolts and other energy projectiles
 - Energy swords collide with other energy swords
 - You can now stop resizing without having to right click the object specifically
 - "Double delay" and "Half delay" type buttons are replaced with a simple number input dialog box.
 - Fire spread radius decreased
 - Replaced fireworks SFX
 - Minor changes to firework particles
 - Fireworks fuse length is now slightly randomised
 - Minor performance improvements
 - Changed blaster impact remnant effect
 - Machine blaster bolt is slightly less bright
 - Made all guns (for humans) much lighter and decreased their recoil
 - Made the submachine gun a little smaller
## Fixed
 - Useless text in mod error description 
 - Red barrels being unreasonably hard to set off
 - Bleeding particles appearing outside the bounding box of the limb
 - Ambient temperature input permanently blocking user input
 - Strange Tesla coil business
 - Tank barrel displacement issues
 - Phenomenal startup times if you have hundreds of Workshop subscriptions
 - Infinite android "blood" amount 
 - A bug where you sometimes couldn't delete a contraption
 - Other minor bugs that nobody hopefully noticed

## [1.17.3] - May 16 2021

## Removed
 - OKAY I REMOVED THE BUG REPORT FORM. Jesus Christ. What is wrong with all of you. Within the first hour of releasing the update, I had to IP ban an embarrassing amount of people. As a side note, please uninstall Sanguinem Triae because about 50% of all the reports I received were caused by it. No offense to its creator, but this is a disaster.

## [1.17.2] - May 15 2021

## Added
 - Temperature unit setting
 - Frozen limbs turn blueish
 - In-game bug report form

## Changed
 - Minor performance improvements
 - Nuclear explosions no longer set everything on fire (necessarily)
 - Nuclear explosions now only burn things in its line of sight
 - Darkened the pause menu
 - Power gauge is less susceptible to heat damage
 - Igniting things via the context menu is more clearly effective

## Fixed
 - Burning-related bugs
 - Strange wire colour bugs
 - Magic purple glow? Probably fixed?? Inform me please
 - Wires on piston head (and other objects) acting weird

## Removed
 - Ignition sound

## [1.17.1] - May 9 2021

## Fixed
 - Weird water bugs
 - Humans not burning for some reason
 - Bleeding not fully stopping when temperature is under 0
 - Insulators no longer catch fire
 - Collision exit bug


## [1.17] - May 9 2021

## Added
 - Basic temperature simulation 
 - Most hot metals glow
 - Heat pipe
 - Thermometer
 - Insulator
 - Hovercar
 - Freezeray
 - Heatray
 - Heating element
 - Cooling element
 - No collision link (Phase link)
 - Framerate limit setting (will only take effect if Vsync is disabled)
 - Bullets slow down and diverge under water
 - Rocket launcher rockets slow down under water
 - Forced resting pose

## Changed
 - Decreased copper wire strength
 - Notifications appear instantly instead of sliding in a little too late
 - Decreased base screen shake intensity
 - Plates are a little less fragile
 - Things burn slower
 - Minor performance improvements

## Fixed
 - Axe serialisation bug (this may break axes in existing contraptions)
 - Potential temporary freezing when you have a lot of undownloaded workshop mods
 - Mods being able to break the mod list
 - A bug to do with sleeping rigidbodies
 - Limb-to-limb energy transfer problems

## [1.16.5] - April 12 2021

## Added
 - Copper wire (destructible conductive wire)

## Fixed
 - The car engine no longer sticks out the car 
 - "OnLoad" will now be called when the mod is activated for the first time. This fixes a few issues.

## [1.16.4] - April 11 2021

## Added
 - Mods that incorrectly call path-dependent functions will now throw exceptions

## Fixed
 - Energy sword save/load issues
 - Energy sword motion blur being invisible at low framerates
 
## [1.16.3] - April 7 2021

## Fixed
 - Screen shake was gone?? It's back now
 
## [1.16.2] - April 6 2021

## Added
 - ModAPI.RegisterInput. Check the wiki for more information: https://www.studiominus.nl/ppg-modding/api/modApi/methods/registerInput.html
 
## [1.16.1] - April 6 2021

## Changed
 - Bleeding particle count increased

## Fixed
 - Ramp charring
 - Energy Sword recoil being too high


## [1.16] - April 6 2021

## Added
 - Energy Sword
 - Bicycle or something
 - Spike grenade
 - Ramp
 - Mods in the mod list now show the errors in their description
 - UI sound when changing tools using keyboard shortcut
 - Beta disclaimer text

## Changed
 - Major texture overhaul
 - Major car overhaul (This will likely break all mods that use them as a base)
 - Bus chairs in busses are less likely to snap off
 - Things are less likely to set each other on fire
 - Slight post processing change
 - Increased machine blaster firing rate
 - Vehicle impact sounds
 - Lasers pass through flasks
 - People can now hold broken glass
 - Impact sounds are more consistent
 - Fire is a little less bright and faster
 - Bleed out from dismemberment is slower, but there is more visible amount of blood
 - Updated to Unity 2020.3.1f1 LTS
 - Fire particles can't be too big :D
 - Hammer is wood
 - Several significant optimisations, especially for inactive objects 
 - Android damage is more apparent
 - Improved help text
 - Changed Gorse damage colours
 
## Fixed
 - Strange shadow on Sea
 - Explosion bug in a specific location on Hybrid
 - World-UI lighting bug
 - Jittering bus chairs
 - Detail mode staying on when certain Workshop contraptions are spawned in
 - Pin tool location bug when pinning humans
 - The camera no longer reacts to input if the mouse is not over the window
 - The camera no longer stops following a target when the window is out of focus
 - The camera will no longer lose sight of a target it's following
 - Flesh wound damage bugs
 - Immobility field selective layer bugs

## Removed
 - Hand tool

## [1.15] - February 24 2021

## Added
   - Empty flask
   - Oil flask
   - Nitroglycerine flask
   - Blood flask
   - Gorse blood flask
   - Blaster rifle
   - Physics gun (has gun in the name but it's actually in Machinery)
   - Grenade launcher
   - New map
   - Bleeding-under-water effects
   - Fog environment option
   - Simplified background rendering option
   - Pressing a tool key again will cycle through the child tools
   - A space above the "quit" button in the pause menu
## Changed
   - Map thumbnails
   - Capped bullet impact force
   - Bubble effect is toned down
   - Sword texture
   - Stick texture
   - Bat texture
   - Increased maximum rotor speed to 8000
   - Human heights are more varied
   - Made sniper rifle more accurate
   - Rewrote laser projectile behaviour
## Fixed
   - Human insane flipping-when-head-touches-ground bug
   - Pin visual location bug
   - Blood tank rendering bug 
   - Minor bugs

## [1.14] - January 24 2021

## Added
   - Rotor
   - Power Gauge
   - Toggleable Mirror
   - Bulletproof Sheet
   - Humongous now has a light source
   - Pin tool
   - Hand grenade now actually shows a pin flying off
   - A little more information in the compiling box
   - Bandages will slowly look soaked in blood
   - Underwater explosion effects
## Changed
   - Panels
   - Some particle effects
   - Energy Vessel texture
   - Fireworks power is scaled with the object scale
   - Hand grenade texture
   - Hand grenade dismembering chance
   - Reorganised tool bar
   - Fancy effects option also toggles many other effects
   - Made electricity particles less intense
   - Made chainsaw less likely to sever limbs
   - Jukebox is heavier
   - General purpose bomb is a little more powerful
## Fixed
   - Some Steam related bugs
   - Many minor bug fixes
   - Weird menu scrolls-to-bottom-on-page-selection bug
   - Performance improvements
   - Notifications no longer block interaction

## [1.13.1] - December 9 2020

## Added
 - Detached Beam Cannon
## Fixed
 - Detached Laser Cannon muzzle flash problem
 - Radio channel sound bug

## [1.13] - December 7 2020

## Added
 - Landmine
 - Chainsaw
 - Detached laser cannon
 - Detached 120mm cannon
 - Signal flare
 - Defibrillator
 - De staf van Sinterklaas
 - You can now right click a wire and delete it. Deleting wires was already possible but it was incredibly unintuitive. This is toggleable.
 - Basic controls are shown on spawned displays when a map is first ever loaded
 - Render scale settings

## Changed
 - A completely different mod compiler
 - Incremental mod loading
 - Unchanged mods won't recompile on startup
 - General purpose bomb is now much more powerful
 - A torch sets things on fire when touched
 - Bandages slowly heal the limb
 - Anti-aliasing settings
 - Windowed mode resolution is remembered
 - Aerial Faith Plate retexture

## Fixed
 - Weightlessness not affecting certain child objects
 - Lots of minor bugfixes
 - Epic water splash performance bug
 - ModAPI.PixelSize is correct now
 - Immobility field irregularities

## Removed
 - The "Force refresh mod list" button is now gone. The safest way to refresh the mod list is to restart the game

## [1.12.2] - November 26 2020

## Added
 - Holographic text display

## Changed
 - Changes to heart rate calculations again
 - New player preferences system. A few settings may have reset to their default value.
 - Removed display resolution options. Just resize the window. Fullscreen mode will default to the native display resolution.
 - Controls tab in the settings menu now shows the key rebind page instead. The scroll sensitivity has been moved to the General tab.
 - Minor changes to particle effects

## Fixed
 - Gentle drag tool dampening
 - Major mod loader issues
 - Infinite propagation signal limit. This will break contraptions that rely on more than 1024 simultaneous signals. Do note that creating an infinite signal loop *will still slow your game down*, it just won't freeze anymore. It actually might still freeze on slower computers but the point is that infinite loops no longer cause memory leaks.

## [1.12.1] - November 6 2020

## Changed
 - Oil can be extracted from androids

## Fixed
 - Fluid dynamics inconsistencies
 - Heart monitor BPM calculations
 - Strange double paste issue
 - Minor optimisations

## [1.12] - October 31 2020

## Added
 - Servo
 - Blood tank
 - Heart monitor
 - Gentle drag tool
 - Blood vessel wire
   - Transfers blood vessel contents from limb to limb
 - Coagulation Syringe
 - Two extra channels for activation signals
   - The new channels will be able to allow machines to perform different actions
 - Signal channel converters
 - All powers now have effects
 - The Winch machine will now toggle an internal battery when activated with a red signal
 - Vehicles reverse their gear when activated with a red signal
 - Electromagnets will reverse polarity when activated with a red signal
 - Option to disable selection outlines
 - Statistics screen
    - Some statistics are stored by Steam. Others will only start counting from this update onwards.
 - ModAPI.RegisterTool&#x3C;T&#x3E; function. This allows modders to create custom tools.
 - ModAPI.RegisterPower&#x3C;T&#x3E; function. This allows modders to create custom powers.
   - You can inherit AOEPowerTool to easily create AOE powers

## Changed
 - Decreased human drown time to 90 seconds (used to be 120 seconds)
 - Icons
 - Humans receive less shock when shot
 - Zombies are no longer immortal and can be killed when severely damaged
   - Extremely damaged dead bodies are unable to be zombified because they wouldn't survive even as a zombie
 - Humans have a small chance to survive severe damage to the head
 - Crossbow texture
 - "Expanded decals" is now "Fancy effects" and will toggle several other effects too (mainly water splash particles)
 - The Gorse is now immune to acid
 - Blood circulation calculations

## Fixed
 - Context menu activation not being a direct activation signal
 - Some EMP related problems
 - Some rendering performance problems
 - Airfoil outline rendering
 - Drag tool inconsistencies
 - Arm flailing when shot in upper chest
 - Local contraption paths. This should make many corrupt contraptions readable again

## Removed
 - Android bleeding

## [1.11.1] - October 2 2020
Lots of ones this time.

## Fixed
 - Contraption thumbnails no longer contain overly bright lights
 - Debris no longer fall through the world
 - Gorse projectiles work again

## [1.11] - October 2 2020
## Added
 - Lighting
 - Torch
 - Flashlight
 - EMP generator
 - Metal pole
 - Wooden pillar
 - Pulse Drum gun
 - CreateLight function in ModAPI
 - Invalid contraption name notification

## Changed
 - Floodlight sound
 - Steel binding is a bit less fragile
 - Stunner effect
 - Anchor texture
 - Workshop contraptions are only loaded once on startup now
 - The Jukebox can now be destroyed
 - Decreased human g-force damage
 - Steel Binding gets weaker the more burnt attached objects are
 - Blood particles are no longer drawn on top of the bounds

## Fixed
 - UI navigation interference
 - Some selection outline issues
 - Minor bugs
 - Performance improvements
 - Unnecessary memory usage
 - Invisible pause menu bug 
 - Wire deletion UI is now drawn over everything else

## Removed
 - Thruster slow startup
 - Valley
 - Flat

## [1.10.2] - September 17 2020

## Fixed
- Enormous serialisation bug

## [1.10.1] - September 17 2020

## Fixed
- Ion bolts not being cleared
- Wire (and more) serialisation issues
- Metal detector inconsistencies

## [1.10] - September 15 2020

## Added
   - Sticky grenade
   - Brick cube
   - Metal cube
   - Metal pyramid
   - Small button
   - Dampening box
   - Conveyor belt
   - Ion Cannon
   - Clamp
   - Settings button
   - Environment options panel (most beta thing about this beta)
   - Clear debris button
   - Fragmentation explosives can more easily dismember limbs
   - Screenshake intensity slider
   - Joint stress indication in Detail view
   - Buttons to enable/disable all mods
   - Indicator whether or not Steam has been properly initialised
   - Electronics tag
   - `IonExplosion` and `Vapor` particle effects have been exposed
## Changed
   - Rewrote nuclear explosion behaviour and redid particle effects
   - Thruster particle effects
   - Thruster textures
   - Shortened thrusterbed warmup
   - Shrunk COM gizmo
   - Decreased range and shockwave intensity of grenades
## Fixed
   - Minor optimisations 
   - Impact force calculations
   - Limb crush calculation
   - Thruster burn area calculation when resized
   - Auto exposure is no longer tied to the time scale
   - Generator particles now scale properly
   - Some audio priority issues

## Removed
   - Generator electricity sound
   - Buttons no longer emit electricity

## [1.9.5] - August 12 2020

## Added
   - Confirmation dialog when attempting to overwrite a local contraption
   - Stormbaan lightning gun
   - (Modding) PhysicalBehaviour.RefreshOutline method that will reset the outline object to the current sprite. This method is also automatically called when the user changes the sprite of an object that uses RandomSpriteBehaviour
## Changed
   - Contraption save screen is now a dialog box
   - Slider has less resistance
   - Destructible cable now has a variable force threshold based on the mass of the attached objects
   - Settings menu is now separated by category
## Fixed
   - Busses are more stable. This will break some older contraptions with busses in them.
   - Debris created by destroyable objects will now properly be removed when undoing their creation
   - Motorised wheel collider is more accurate now
   - Motorised wheel no longer causes inaccurately serialised wires
   - Fixed the godforsaken car texture
   - Steel binding not being broken by lasers and Beam rifle beams

## [1.9.4] - August 2 2020

## Added
   - OnLoad method for mods. This is a static method that will be invoked after all mods are loaded. This is unlike the Main method which is invoked when the catalogue is populated.
   - ModAPI debug drawing feature
   - ModAPI.PixelSize constant
## Changed
   - Updated to Unity 2020.1.0f1
   - Fire looks better when moving fast
   - Beam Rifle texture
   - Beam Rifle recoil increase
   - Decreased bullet drop
   - Decreased bullet impact sound volume
## Fixed
   - Minor bug fixes

## [1.9.3] - July 23 2020

## Added
   - Slight bullet drop
   - Tracer speed based on actual round speed
   - ModAPI.Register&#x3C;T&#x3E;
      - This function accepts a generic type parameter that derives from MonoBehaviour. These components will be created in and will exist from map load to map unload. You can use these to run scripts in the background.
   - PhysicalProperties.LodgeStrengthMultiplier
      - This field determines how difficult it is to pull the object out if it has been lodged into something. It is set to 1 by default.
## Changed
   - Slipperly soap
   - Androids are now 
   - 120mm cartridge is now 30mm
## Fixed
   - Timed Gate bug
   - Tracer resize bug
   - Tracer water bug
   - Mod active status change when mod updates
   - Bullets hitting their origin weapon
   - Minor performance improvements

## [1.9.2] - July 21 2020

## Added
   - Bullet tracer option
   - Minor addition to firearm sounds
## Changed
   - Machine gun now fires ballistic rounds with tracers
## Fixed
   - Hidden achievement is now achievable for older players
   - Mod loading problems for some
   - Minor performance issues
## Removed
   - That loading screen only caused problems apparently so that's gone forever

## [1.9.1] - July 17 2020

## Changed
   - Angular and translational snapping is now world-based
   - Androids have tougher armour
   - Sliders now have a 0-100 limit
## Fixed
   - Chain explosives no longer cause immense lag because of the un-fixed bug

## [1.9] - July 17 2020

## Added
   - Plank
   - Winch machine
      - Power it to make it move
      - Activate to toggle direction
      - Change limits in context menu
      - See limits visualised in Detail view
   - Radio activation signals
   - Soap
   - Slider
   - Industrial Gyrostabiliser
   - Angle snapping (hold LAlt while rotating in paused mode)
   - Translation snapping (same goes for unpaused)
   - "Set angle" context menu option
   - Legacy tonemapping setting
   - Nearly useless short loading screen
   - Hidden achievement
   - Added "pixelated" parameter to ModAPI.LoadSprite
   - Added ModAPI.LoadTexture to load textures without a sprite attached
   - Added a friendly helper function to make changing human/android/gorse texture swapping easier. See the snippet page for more information. https://github.com/mestiez/ppg-snippets
   - Also made it easier to change procedural damage colours such as bruises.
## Changed
   - Humans bleed out faster
   - Updated Steamworks․NET and the Post Processing Stack
   - Gyrostabiliser is a little more powerful by default
## Fixed
   - Malformed mods should no longer prevent other mods from working
   - Drag force is now proportional to object mass to prevent unnatural physics events
## Unfixed
   - Due to popular demand, explosives can now be detonated multiple times

## [1.8.1] - June 30 2020

## Added
   - Mod list now automatically updates itself when during runtime. You do not need to restart the game.
   - In case Steam sends the message too soon (before download), there is a "Force reload" button.
## Changed
   - Springs no longer reset their length when moved in paused mode.
## Fixed
   - Dumb problem in RandomSpriteBehaviour (my most sincere apologies to riceworld)
   - Fixed Gate not sending initial activation signal occasionally
   - Wire length miscalculation

## [1.8] - June 21 2020

## Added
   - Mod workshop support
   - Mod tag support
## Changed
   - URLs opened in-game now open in the Steam overlay when possible
   - Made bullet water impact a little less dramatic
   - Rewrote bullet "physics" calculation
   - Jukebox glows brighter the more energy it has
## Fixed
   - Wood struts no longer look weird
   - Many problems to do with bullet physics are gone

## [1.7.3] - June 18 2020

## Added
   - Overcharged jukeboxes now destroy heads
   - ModAPI.CreatePhysicalObject
   - Rotted humans are more stiff now, just like in the pre 1.2.2 days.
   - The Jukebox now supports MP3 files
   - ^ also goes for ModAPI.LoadSound

## Changed
   - Bones are less easily broken
   - Living beings are just a little more durable overall
   - Gyro stabilisers now scale their strength with their size
   - Added back in the beta sounds for the LMG
   - ModAPI.Notify now accepts any object and prints it as a string
   - Adrenaline syringe lasts 20 times as long

### Fixed
   - Fixed some business regarding Steam and launching the game from the .exe directly
   - Legacy wires are no longer super dark blue
   - Adding a PhysicalBehaviour manually no longer causes many ObjectReferenceExceptions because there is no inspector to initialise the empty fields.

## [1.7.2] - June 17 2020

### Added
   - "No mods found" message

   - ModAPI.OnGunShot event
   - ModAPI.OnDeath event
   - ModAPI.OnDeath event
   - ModAPI.FindPhysicalProperties function
   - ModAPI.FindMaterial function
   - ModAPI.CreateParticleEffect function

   Visit the documentation for more information

   https://www.studiominus.nl/people-playground-modding
### Fixed
   - ModAPI.FindCartridge bug that nobody would've noticed
   - ModAPI.LoadSound now allows both stereo and mono audio
   - WireBehaviour.SetColor now sets the persistent colour as well
   - Setting the sprite of a burnable object via mods is now reliable
   - Bandages now render on the correct layer

## [1.7.1] - June 16 2020
Small mod API patch

### Added
   - ModAPI:
      - Resource caching
      - FindCartridge
      - LoadSound
      - Notify
      - OnWireCreated
      - OnItemSpawned
      - OnItemRemoved
      - OnItemSelected
      - OnItemDeselected
      - OnItemActivated
      - GameObject.FixColliders()
   
   - Added some friendly functions that are best showcased on the code snippet page
   
   Visit the documentation for more information

   https://www.studiominus.nl/people-playground-modding

   New useful code snippet page

   https://github.com/mestiez/ppg-snippets
### Changed
   - Default mod texture
### Fixed
   - Improved how mods are loaded and how they are given an error state
   - Inactive mod chaos
   - Multiple bugs in the mod loader

## [1.7] - June 14 2020

### Added
   - Attraction god power
   - Repulsion god power
   - Lift god power
   - Pyrokinesis god power
   - Copy/paste shortcuts
   - Pink explosive
   - Pink syringe
   - Adrenaline syringe
   - Light machine gun
   - Shock detector
   - Spring wire
   - Bandage wire (stops bleeding)
   - Expanded decals option
   - Specific round casing textures
   - Experimental mod support
      https://www.studiominus.nl/people-playground-modding
### Changed
   - Separated tools and god powers
   - Minor changes to black hole
   - General Purpose Bomb is now impact-sensitive
   - Missiles are a little more powerful
   - The missile will now compensate a moving target's velocity for more accurate seeking
   - Changes to how bullet speed falloff is calculated
   - Increased bleeding particle intensity
   - Improved how the decal system works internally
   - Wire rendering optimisation
   - Fire extinguisher now updates visual state of burning object immediately
   - "Flamethrower" now updates visual state of burning object immediately
   - Decreased Handcannon knockback
   - Minor changes to machine gun and tank sfx/vfx
   - Logs have their own folder now
   - Increased firearm range
### Fixed
   - Incompatible contraptions will no longer destroy the entire toybox
   - Game shows info popups instead of letting the toybox crash when deleting a corrupt contraption
   - Firearms are no longer inaccurately inaccurate
   - Lightning power no longer makes noise when over UI
   - Humans and (especially) androids are a little stronger. This should fix their weird behaviour when it comes to walking that as caused by increasing their weight.
   - Increased performance of decal rendering
   - Increased performance of other sprite rendering
   - Missile Launcher range extended
   - Launched missile going through objects in discrete mode
   - Gorses are a little better at aiming
   - Fixed unnecessary CPU usage on idle objects
   - Fixed audio issues introduced in 1.6
   - Clearing everything actually clears everything now
   - Fixed spinny projectile problem
### Removed
   - Sprite deformation (◞ ‸ ◟)
   - Toolbar toggle shortcut is now merged with the toybox toggle shortcut (tab by default)

## [1.6] - May 1 2020

### Added
   - Added workshop tag support
   - Gorse
   - Metal wheel
   - Brick wall
   - Concrete wall
   - Lightbulb (texture concept design by sv1t)
   - Activation gate
   - Activation fuse
   - Machine blaster
   - Missile launcher
   - Silver texture for the I-Beam
   - Steel binding, a destructible metal fixed cable
   - Toybox filter (search bar)
   - Blast marks
   - Information page on main menu shows a little more information
   - The jukebox supports the power of the Industrial Generator
   - Better rocket launcher effects
   - Blasters glow
   - Blasters have recoil
   - Bullets can now ricochet (chance of this happening is based on material hardness and impact angle)
   - You can now toggle decal rendering (disabling will increase performance especially on lower end systems)
   - Detail view now shows the size of the selection box
   - Added a sprite to launched rocket launcher rounds
### Changed
   - Wooden struts look more like planks now
   - Joint stress sounds play less frequently
   - Limbs can only be crushed by guns when Limb Crushing is enabled
   - Machine gun texture
   - Sentry turret now fires a 5.56 round at a lower fire rate, instead of a 9mm at a high fire rate
   - Beam Rifle texture
   - Blast Radius texture
   - Humans are a little less soft
   - Major changes to how bullet penetrability is calculated
   - Android oil is now black
   - Humans are a little more difficult to dismember
   - Log files are now created in the menu as well
   - Improved rendering performance of the immobility forcefield
   - Redid all default jukebox music
   - Camera shake behaves more consistent
   - Explosion sound effects
   - Wood sound effects
   - Blaster is more accurate
   - Machine gun sound
   - Nuclear bomb shockwaves now destroy destroyable objects
   - Resolution list is now a grid
   - Humans are now more realistically sized
   - Lord Talon demanded the fire extinguisher be moved into the "Firearms" category
   - Updated Unity version
### Fixed
   - Pistons will extend properly when resized
   - Charged particles will correctly appear after deserialisation
   - Resize handles will now properly encapsulate the selected objects
   - Bones will break properly when forcefully put in an unnatural position again. For some reason this bug went unnoticed for months.
   - Battery powered lasers will no longer vaporise bodyparts
   - Fire extinguisher and other particles will no longer appear under just decals
   - Resizing weight bug
   - Key triggers won't activate when the UI is blocked anymore
   - Line rendering bug that was causing performance problems when using very old contraptions

## [1.5] - March 25 2020

### Added
   - Immobility Field
   - Reconstructor
   - Rigidifier
   - Wing
   - Propeller
   - Balloon
   - Key Trigger
   - Industrial Generator (dangerous as hell, I'm not sure if this should actually be in the game)
   - Red barrels
   - An unreasonably large map
   - _Detail view_: shows blast radii, limb health, center of mass, and visual center
   - Blood decals are now created behind exit wounds
### Changed
   - Human flesh texture
   - Gut texture
   - Minor changes to the fan texture
   - Changes to explosion effect
   - Increased sensitivity of motion sensor
   - Minor tracer colour change
   - Syringe injections no longer cause wounds
   - Blood particles and other bloody things
   - Sentry turret now aims to heaviest limb in view
   - Revolver (and future weapons with a 38 Special cartridge) is now a little more powerful
   - Acid spreads slower
   - Zombies are a little more... stable
   - Increased bleeding particle rate
   - Increased bleeding particle normal offset
   - Slight tweaks to aerodynamic calculations
   - Syringes now propagate through connected limbs, and their effects linger even when the syringe is removed (this changes all syringe behaviour)
   - Life syringes last for a shorter time 
   - Ultra strength syringe no longer generates electricity
   - Ultra strength syringe effect stacks
   - Explosives might set off nearby explosives
   - Some explosives will now go off when on fire
   - Limb status view is replaced by the _Detail view_
### Fixed
   - Crystals are no longer attracted to magnets
   - Sharp entry bug
   - Android no longer has invisible guts
   - Mass is yet again serialised
   - Minor (de)serialisation bugs to do with the expanded gore stuff
   - Toybox order chaos no longer occurs when Steam isn't running
   - Lasers and detector beams will now functionally pass through glass
   - Bullets will go through syringes
   - Explosives can no longer go off multiple times

## [1.4] - February 26 2020
A small update adding a few new items and fixing a number of bugs following 1.3
### Added
   - Timed gate
   - Glass pane
### Changed
   - Lagbox texture
### Fixed
   - Sentry Turret debris gun is once again functional
   - Stabbing entry vector miscalculation
   - Minor firearm bug

## [1.3] - February 24 2020
### Added
   - A single extra firework variant
   - A set of bells ranging from C4 to C5
   - Structural metal pole thing
   - Siren
   - Propagation wire glows when an activation travels through it
   - Tiny map 
   - Limbs can now explode when hit with overwhelming firepower
   - Resizing
      - Right click an object, select resize. Two handles will appear, one for each axis.
      - Hold shift (or what you have assigned to "rotate faster") to resize in both axes simultaneously.
      - Limited to uniform scaling when resizing many objects at the same time
   - Risky expanded gore mode
      - Adds a number of organs and reintroduces guts to the game. This option is disabled by default and should stay disabled considering the performance impact and limited support / attention. Enable at your own risk :)
### Changed
   - The majority of all machinery is now destructible and will generally cease all function when destroyed
   - Behaviour of aerodynamic objects
   - General Purpose Bomb is now aerodynamic
   - Atom Bomb is now aerodynamic
   - Intensity of plate debris rotational force
   - Firearms now have properties that better reflect their real life version
   - Cathode lights will now shatter when hit with the Beam Rifle and explosions
   - Piston textures
   - Cathode light texture
   - Car textures
   - Barrel texture
   - Sentry Turret texture
   - Lagbox is now gray to indicate its actually made of metal
   - Desaturated blood
   - Context menu has a scrollbar
   - Propagation wire is thinner and looks different
   - Increased maximum double click time for map thumbnails
   - Black hole sound
   - Muzzle flash brightness and resolution
   - New sounds for nearly all traditional firearms
   - New tank shot sound
   - New machine gun sound
   - Disabled fake reverb
   - Metronomes and detectors will no longer propagate direct activation signals (zero propagations away from user iniatiated activation)
   - Versioning will from now on go 1.3 -> 1.4 -> 1.5 and so on
### Fixed
   - Infinite fireworks activation
   - Incorrect cathode light weightlessness effect position 
   - Incorrect broken plate highlight
   - Incorrect broken plate spawn position
   - Giant wooden bowl not looking burnt after being burnt
   - Disassembler muzzle flash is no longer gigantic when weightless
   - Cancelling saving a contraption is no longer broken
   - You can once again pan while hovering over the toybox panel 
### Removed
   - Metronomes no longer burn when energy flows through
   - Cathode tube lights don't make take mass away from their surroundings when shot anymore

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
   - Normal hand grenades are now less powerful
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
   - 9mm Pistol
   - Handcannon
   - Soviet SMG
   - M1 Rifle
   - G1
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
   - This also means the lethality of wounds is now based on how deep it is. Syringe wounds heal quickly, while a spear through the stomach won't heal at all.
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
 - Removed arrow on motorised wheel since every wheel is now reversible

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
- Doubled limb breaking threshold
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