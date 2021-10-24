# The Matrix: Path of Neo (PC) Framerate Fix

This patch is based on ThirteenAG's Widescreen Fix as a base to replace three values in game's memory (frametime delta, time scale, frame rate target).
The values themselves were either taken from known PCSX2 cheat codes (time scale, frame rate) or discovered by me using Ghidra + Cheat Engine (frametime delta, seems to be exclusive to the PC version).

Please see the link below for more information about the original fix.

https://github.com/ThirteenAG/WidescreenFixesPack

# Disclaimer

This fix has not been thorougly tested yet - I can provide no warranty for what happens to your game installation or PC when using this patch.
So far I have played a level without any gameplay glitches that I could see. See the video linked below if you'd like to see the patch in action.

https://www.youtube.com/watch?v=lR_j6N7Dy4E

# Installation

Place dinput8.dll and the "scripts" folder into the root of your Path of Neo installation folder.
Check scripts/TheMatrixPathOfNeo.WidescreenFix.ini for screen resolution, aspect ratio and framerate fix settings.

# Building

To build the patch yourself, see ThirteenAG's instructions for their original widescreen fix. 
Replace their original dllmain.cpp with my version to add the framerate unlocking functionality.

# Future plans

When running on modern hardware, the game exhibits graphical glitches on modern hardware. 
For now, I suggest turning down the quality setting (in MatrixConfig.ini in the root folder of your game) down to 8 to avoid major lighting system glitches.
The "doubling"/haze effect will still exhibit issues (separation too great), same goes for character skin shading. 
I will look into resolving this issues when I have the time for it.
