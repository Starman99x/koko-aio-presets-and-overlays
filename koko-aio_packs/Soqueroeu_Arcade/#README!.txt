ALL presets depend on "Arcade_(Main).slangp". This means you should not rename or delete it, but you can adjust all presets at the same time by editing the contents of the main preset (with any text editor).

For example, you can replace the main preset with the alt "no-bloom" version that I included in a separate folder to disable bloom in all presets properly (always keep backups).

Or you can change the CRT mask type to Slotmask by replacing this refrence line:

#reference "../../shaders_slang/bezel/koko-aio/monitor-bloom-bezel.slangp"

With this one:

#reference "../../shaders_slang/bezel/koko-aio/monitor-slotmask-bloom-bezel.slangp"

If you want to both remove bloom and use a slotmask main preset, then first use the alt no-bloom main preset as mentioned, open it up, and replace this line:

#reference "../../shaders_slang/bezel/koko-aio/monitor-BASE.slangp"

With this one which refrences a slotmask default preset by kokoko3k:

#reference "../../shaders_slang/bezel/koko-aio/monitor-BASE.slangp"

You can do other things like disabling the spot and vignette to squeeze more performance by changing these overrides to zero:

DO_VIGNETTE = "1.000000"
DO_SPOT = "1.000000"

They become like this:

DO_VIGNETTE = "0.000000"
DO_SPOT = "0.000000"

Experiment as you like.