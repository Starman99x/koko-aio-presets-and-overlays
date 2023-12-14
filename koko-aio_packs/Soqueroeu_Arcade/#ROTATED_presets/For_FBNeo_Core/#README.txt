When loading some vertical aspect ratio games with FBNeo core, the texture image.png might get flipped in a wrong direction, to fix this problem, I had to rotate the texture images. And add an image rotation override to the shader:

BG_IMAGE_ROTATION = "-2.000000"
S_POSITION_X = "0.500000"

If your game is not affected by this problem, then use the "Reverse_fix" presets in the other folder.

There's also a diffrent Global Shift/Zoom parameter between fix and reverse fix versions:

fix: GLOBAL_OFFX = "0.060500"
reverse: GLOBAL_OFFX = "-0.060500"

These are some games affected by this issue:

- Circus Charlie (level select, set 1)
- Contra (US / Asia, set 1)
- Donkey Kong (US set 1)
- Donkey Kong Junior (US set F-2)
- Donkey Kong 3 (US)
- Detana!! Twin Bee (Japan ver. J)
- Final Star Force (USA)
- Galaga (Namco rev. B)
- Galaxian (Namco set 1)
- kiKi KaiKai
- Mappy (USA)
- MS Pacman
- Pac-Man (Midway)
- Pooyan
- Spy Hunter
- Star Force
- TwinBee (ROM version)

And these are some games that are NOT affected by this issue:

- 1941 - Counter Attack (900227 World)
- 1942 (Revision B)
- 1943: The Battle of Midway (Euro)
- 19XX - the war against destiny (960104 Euro)
- Ikari Warriors (US JAMMA)
- Punch-Out!! (Rev B)
- Q*bert (US set 1)
- Q*bert's Qubes
- Qix (Rev 2)
- Qix II (Tournament)

I think it's a matter of wether a game is originally rotated by 90 degree vs 270 degree.