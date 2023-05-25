it seems that MAME core (current) does not automatically switch to vertical aspect ratio when using koko-aio shader, since koko-aio itself requires RetroArch aspect ratio to be set to full, and this seems to cause a conflict with how mame handles the aspect ratio, to fix this, I added this override to all presets:

ASPECT_X = "-6.000000"

If you are instead, using MAME 2003-Plus or a diffrent MAME version, you might need to reverse this override to default:

ASPECT_X = "0.000000"

Or try the other presets in FBNeo core folder.