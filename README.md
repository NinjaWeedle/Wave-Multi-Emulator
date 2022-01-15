# Wave-Multi-Emulator
A Multi-System emulator in Scratch 3.


This is the official repository for Wave Multi-Emulator. More info on Wave can be found here: https://scratch.mit.edu/studios/27152609/

If you are looking for information on the HyperWaveCHIP-64 extension for CHIP-8, look here: https://github.com/NinjaWeedle/HyperWaveCHIP-64


Changelog:

V0.7.X:
V0.7.9: Fixed a variety of audio issues with Chip-8 that caused audio to not play in any CHIP-8/SCHIP games, and also added debug info to the pause menu.
V0.7.8: Add very early Mega-Chip support.
V0.7.7: Fix hi-res CHIP8 games taking forever to load.
V0.7.6: Add Boot-128 support, Fix bitshifts not setting VF correctly in CHIP-8
V0.7.5: Update DualGB to Early GBC build.
0.7.4: Major GUI overhaul, add BBC micro:bit integration. CHIP8: Change 00F0 to 00E1. Goddess A: Minor updates to CPU structure. GBA: ROM importer fixed.
0.7.3: GUI update by @Executec
0.7.2: bugfixes
0.7.1: CHIP-8 FFT speedup, Bugfix on edge case with DXYN VF collision, fix 8XYD/8XYF
0.7: Added Cool NES Emulator by @GenericHeroGuy, added 1s1s Bytepusher by @52525rr,
added 2 new options for themes, fixed WAVE-8 crashing in vanilla scratch occasionally,
fixed theme switch crash, added sounds when clicking the on screen arrows in the menu,
removed N64 icon, added GUI to rom importer, fixed GBA rom importing.

V0.6.X:

0.6.20: bugfixes, add 00F2, F100, F200, F300, 8XYF
0.6.19: (CHIP8) Fix palette swaps
0.6.18: (CHIP8) Add screen invert instruction 
0.6.17: Fix SuperNeatBoy falling thru the floor.
0.6.16: Added OR mode drawing.
0.6.15: CHIP8 Scroll left issue fixed.
0.6.14: Create new instruction for WAVE-8, FN03
0.6.13: Update HyperWaveCHIP-64
0.6.12: Implement HyperWaveCHIP-64 extension.
0.6.11: Add some HYPERCHIP-64 opcodes
0.6.10: Added Screen and Audio toggles to CHIP-8.
0.6.9: Add audio support to CHIP8, fix scrolling bug.
0.6.8: CHIP8: Add visible PC Counter
0.6.7: Fixed Long I skips, made quirk changes stay enabled/disabled until page reload 
0.6.6: Improved CHIP-8 Audio
0.6.5: scroll instruction updates
0.6.4: Two new one-pass drawing methods for CHIP-8: One by @Kouzeru (Sharp mode), and one based off the original (Legacy mode)
0.6.3: Bugfixes.
0.6.2: "Import State" button relocated. GB: The game title is now shown at bottom of the screen.
0.6.1: GB: bugfixes. CHIP8: Keypad clones are now cleared upon emulator reset.
0.6: GB: @52525rr's As-of-yet-unnamed Gameboy emulator has been added!
CHIP-8: Mobile support for the CHIP-8 Emu has been added,CHIP-8 games now render correctly, Brand-New WAVE logo rom by @AArt1256 added as the default rom, screen position moved to top.

V0.5.X:

0.5.6: Certain SCHIP-era games now display their  titles when run in SCHIP mode.
0.5.5: GUI bugfixes. CHIP8: CGA0 colors are now used. Arrowkeys now supported.
0.5.4: CHIP8: New drawing method.
0.5.3: CHIP8: New audio system, implemented pitch changes
0.5.2: some GUI updates such as allowing the user to press enter/space to start an emulator, added support for the "Goddess A" fantasy computer (Still a WIP).
0.5.1: CHIP8: FINALLY. FIXED. THE KEYBOARD BUG.  Also fixed scrolling in plane 0.
0.5: CHIP8: ADD XO-CHIP 1.1 SUPPORT (no audio). Add multiple plane drawing, Remove option to disable wrapping and collisions, replace it and HPS slider with dedicated button to Switch between XO-CHIP and SCHIP Compatibility mode.

V0.4.X:

0.4.9: Implement Fx3A to prepare for XO-CHIP 1.1's updated audio system
0.4.8: Made changes to make the menu operate smoother in 60 fps mode. CHIP8: press 0 to disable Wrapping and collisions. Toggle this on and off again once you move past the outer edge to fix "Ant: The Search for Coke".
0.4.7: Some minor progress on Game Boy.
0.4.6: - CHIP8: When run in Turbowarp, the draw mode now defaults to "Accurate" instead of "Fast."
- UHWEI: Fixed preloaded ROM loading.
- General: Made several menu performance improvements. Added dev script to fix saving that deletes unused DS and GBA lists.
0.4.5: Fixed DS ROM importing, added new animations to menu.
0.4.4: Added option to draw every frame in CHIP8 (fixes sound timing issues) Made small changes to 3DS background.
0.4.3: NDS and GBA roms now display their titles when running, Made a few small graphical updates, further improvements to project stability to improve the user experience.
0.4.2: Chip8: Added vertical half-pixel scroll support, removed Scratch double speed mode as it made some games unplayable. UHWEI: added function to set Chip8 start address: Type "set start address" and then type what address chip8.pc should start at. May be useful for chip8x.
0.4.1: Updated GBA emulator backdrop, made a few preparations for Gameboy and GBA
0.4: - General: Added Geotale's DS Emulator v0.1.1.3, added Turbowarp support, added 1 new music track, added some portions of the Gameboy emu, minor graphics updates.
- CHIP8: Added XO-CHIP support (no sound buffer 
 or color support yet), fixed the SuperChip and Hi-res chip8 incomplete draw bug, optimized drawing to increase speed, removed 00FA.

V0.3.X:

0.3.11: Added 00DN (XO-CHIP), 5XY1 (CHIP8E), and 00FA (chip8run). Preparing for XO-CHIP.
0.3.10: Fixed a bug causing DXYN to not render correctly in 128x64. Added a toggle to set VF to 1 if FX1E results in an overflow (Spacefight 2091! and SC test rely on this behavior)
0.3.9: Fixed 00CN, brought project size down to under 5MB, miscellaneous optimizations. Added pong 2 to the list of included roms- type "Load Pong 2" in UHWEI to play!
0.3.8: Final schip instruction (00CN) added, display optimizations, timer speed doubled to the correct rate of 60hz, fixed bug that caused Chip-8 emulator to still run in the background after 00FD is called, compressed music to reduce filesize.
0.3.7: DXY0 has been fixed- making (some) SCHIP games finally playable! 
0.3.6: CHIP8: Added option to enable and disable VIP style jumps when you press enter. Defaults to VIP, but setting it to 0 enables SCHIP-style jumps (BXNN). Removed the toggle to manually change screensize (It was useless anyway)
0.3.5: You can now set the CPF in chip-8 by pressing space.
0.3.4: Fixed Shift Quirk
0.3.3: Fixed Subtraction in CHIP8, SCHIP support is almost there, added left and right scrolling. Game Boy: added bits and pieces from Geotale's livestream, no code runs.
0.3.2: Added experimental hi-res chip8 support. hi-res games should load but won't render the full 64x64 resolution yet. Made the beep sound an actual beep as "ping bing" was a bit grating
0.3.1: Added Chip8 rom loading commands (using only public domain roms) to UHWEI for easy loading.
New Commands to try: "Load Rocket Launcher", "Load 1P Pong", "Load Breakout"
0.3.0: 
   Misc: Implemented Executec's expanded themes system, removed useless MetaNES variables.
   Chip8: fixed cycle bug, fixed Chip-8 keyboard bug, COSMIAC VIP accurate sound timer added, FX75 and FX85 implemented. Preparing for full SCHIP support.

V0.2.X:

0.2.2: just fixed exit opcode and removed other stuff from 0.2.2B.
0.2.2B: added an option to disable exit opcode (now disabled by default, can be reenabled by typing "exitop" in UHWEI)
0.2.1: fixed more keyboard bugs, fixing compatibility with Tetris and Keypad Test.
0.2.1B: Keyboard works now! Added 2 SCHIP opcodes as well as shift quirk support.
0.2.0: You can now press enter to reset the chip-8 emulator. Use the speed slider to speed up  or slow down chip-8 Untested Chip 8 quirk support- reset to bring up their sliders. (Only the load_save quirk is currently implemented)
0.2.0B: Chip-8 is 98% working! ALL opcodes are functional! I just need to adjust for rom quirks and speed.

V0.1.X:

0.1.9: DXYN WORKS NOW! Only fx33 needs fixing still, but then we'll have a fully working Chip-8 Emulator!
0.1.9B: minor chip8 stuff. Theme importer can now correctly handle when someone inputs nothing.
0.1.8: Changed the way the sound engine works to boost speed. Added a VMU emulator base.
0.18B: Added an "exit" Command to UHWEI. Minor menu bug fixes. Added "reset" and "get_keyboard" custom blocks to the GB emu.
0.1.7- Fixed themes- Wave now restarts when you import a theme. entering nothing or entering zero will cause the theme to revert to the default 1111 theme. WDS Theme added! (2211)
0.1.7B- Added theme support- details inside in backdrop. Added a (currently unused) function to the GBA emulator. Changed the menu system to allow exiting emulators. Nearly finished listing what all the opcodes are inside the Chip-8 emulator.
0.1.6B- Added credits and other hidden commands to UHWEI. Removed the note about NDS rom importing as it is broken and no NDS emulator is included yet. Combined the Gameboy sprite with the background and removed sprite8.
