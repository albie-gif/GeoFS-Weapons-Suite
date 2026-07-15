## GeoFS-Weapons-Suite
Separate userscripts, still in development, which create visual weapons systems for GeoFS flight simulator. Non-multiplayer, this suite includes tracking missiles, guns and bombs, as well as the HUD found in my HUD repository. 

# Instructions for use:
Each of these scripts should be used as a separate Tampermonkey userscript. Load in GeoFS and fly. 

# AI declaration:
Made with extensive use of AI (Microsoft Copilot). 

# Declaration of own work:
Replacing the ad banner was achieved by deriving content from https://github.com/AirplanesAviation2361/Geofs-Ad-banner-changer-v1.3
Everything else is myself + AI. 

## SCRIPTS:

# GeoFS HUD v5
Install first. Shows crosshairs, CCIP and turn actualiser. Activated/deactivated by HUD ON/HUD OFF switch on right. Includes code to obscure ad panel and replace with a black background for other HUD informatics. 
- Known bugs: CCIP is not accurate to bombs script. 

# GeoFS Bombs v5
A bomb counter will appear on the right side of the screen, reading 'BMB 12 AGL ---'. Press comma "," to release a bomb. The bomb counter will count down to 0 then show EMPTY. The AGL counter will show the distance between the bomb and the ground. When the counter shows EMPTY, press and hold comma "," for five long seconds and the bomb count will reset to 12.
When a bomb is released, there is a flash to indicate its release, then a thick smoke trail will follow the bomb. Upon impact, an explosion in orange and black is shown, then smoke is released lasting 20 seconds. A black scorch mark will remain in place. The scorch marks last until game reset or until the number of bomb scorch marks exceeds 100.
- Known bugs: steeper hills are not necessarily recognised as ground, and bombs may explode below them; bombs dropped into water while water effect is enabled may not ever explode. 
- Upcoming developments: sounds.

# GeoFS Gun System v8
Press slash '/' to fire. Bullet visuals should appear from either wing. The observant will note that at low altitudes small black scorches are briefly visible at impact sites when the ground is fired upon (can only be seen at low altitude).
- Known bugs: guns are not well aligned to aircraft; guns will not fire if aircraft is rolled more than around 60 degrees; bullet visibility is poor; tracers are semi-static
- Upcoming developments: sounds, better tracers, impact recognition on aircraft.

# GeoFS Target Tracker v10
When run, a button will appear on the right of the screen reading "MA OFF", and in the top right a panel also reading MA OFF. If the button is clicked, the panel will show a green bar and read "NO TARGET" until there is an aircraft in view. If aircraft are visible on the screen, one (usually the nearest) will be marked with a green diamond and bar, and the panel will show "TRACKING" and the plane's name, coordinates, range and number within the available targets. After 3 seconds, the bar and diamond will change to red (the bar incrementally) and the panel will show "TARGET LOCKED". At this point, if the missile system is enabled, a missile fired will track this aircraft. Click "Y" and "SHIFT + Y" to cycle through available target aircraft. If the aircraft goes out of view, the lock will be lost and an arrow and "TGT" will appear indicating the direction. 
- Known bugs: TGT -> tracker is not reliable when the aircraft is more than 90 degrees from your field of view; missiles stay locked after aircraft leaves FOV lock radius having been previously locked.
- Developments: lock and target acquisition sounds; make nearby aircraft lock faster than distant ones; prioritise selection for nearby aircraft. 

# GeoFS Missile System v2
Works in conjunction with the Target Tracker (and not without). If MA is on and an aircraft is locked (red diamond), pressing full stop "." (period) will trigger the release of a missile, which will track the aircraft. Upon contact an explosion will be seen with smoke lasting 12 seconds and a permanent black scorch mark (up to 200 scorch marks). 18 missiles can be fired
- Known bugs: missiles will still follow aircraft if targeted but not locked having been locked.
- Upcoming developments: sounds, visuals.

# GeoFS Flight Data Block
Throwing this in for good measure. A block appears in the right HUD panel showing digital values for speed (SPD), altitude (ALT), altitude above ground level (AGL), vertical speed (V/S) and G-forces (G). Values are approximated based on aircraft location data, so are not perfectly accurate (though more accurate than using analogue dials for landing, for example).
- Known bugs: none. 
