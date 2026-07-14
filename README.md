# GeoFS-Weapons-Suite
Separate userscripts, still in development, which create visual weapons systems for GeoFS flight simulator. Non-multiplayer, this suite includes tracking missiles, guns and bombs, as well as the HUD found in my HUD repository. 

# Instructions for use:
Each of these scripts should be used as a separate Tampermonkey userscript. Load in GeoFS and fly. 

# AI declaration:
Made with extensive use of AI (Microsoft Copilot). 

# SCRIPTS 

# Bombs v5
A bomb counter will appear on the left side of the screen, reading 'BMB 12 AGL ---'. Press comma "," to release a bomb. The bomb counter will count down to 0 then show EMPTY. The AGL counter will show the distance between the bomb and the ground. When the counter shows EMPTY, press and hold comma "," for five long seconds and the bomb count will reset to 12.
When a bomb is released, there is a flash to indicate its release, then a thick smoke trail will follow the bomb. Upon impact, an explosion in orange and black is shown, then smoke is released lasting 20 seconds. A black scorch mark will remain in place. The scorch marks last until game reset or until the number of bomb scorch marks exceeds 100.
- Known bugs: none.

# Guns v8
Press slash '/' to fire. Bullet visuals should appear from either wing. The observant will note that at low altitudes small black scorches are briefly visible at impact sites when the ground is fired upon (can only be seen at low altitude).
- Known bugs: guns are not well aligned to aircraft; guns will not fire if aircraft is rolled more than around 60 degrees; bullet visibility is poor; tracers are semi-static

# Target Tracker v3
Description...
- Known bugs: TGT -> tracker is not reliable when the aircraft is more than 90 degrees from your field of view;                                    
