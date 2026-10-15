# Changelog

Updates to the Sonic 1 PS1 ISO Builder, newest first. To get an update, rebuild your disc image with the new
version of the builder (same steps as in the [README](README.md)).

## The disc's executable is named after the game (October 2026)

- The disc now boots **`SONIC1.EXE`** instead of `PSX.EXE` (the `BOOT` line of `SYSTEM.CNF`).
  Emulators and optical drive emulators that show a disc's executable name now show the game's. Nothing in the
  game itself changes.
- The image's SHA-256 changes with it (the new value is in the README's Output section).

## Earlier updates (October 2026)

- **No freeze if the CD drive stops answering:** at a 1-up, the pause menu or a load, the game used to wait for the
  drive forever; it now asks again after a few seconds and carries on.
- **Delete a save file:** on the save select, press Select on a used file and confirm "Delete Saved Game?" (as the
  mobile versions' Delete button). The other files, the Time Attack records and the settings stay.
- **Marble Zone's lava flow** no longer flickers (some of its frames were missing from the video RAM).
- **The credits' last screen** draws the 7th emerald (it was missing when the 7th emerald setting is on).
- Green Hill's waterfall sounds now play (they were left out of the zone's sound set).
- **Sonic 3 shields and the insta shield:** the original 2013 release's hidden shield setting is now in Options
  (Shields: Sonic 1, Sonic 2, Sonic 1 + S3, Sonic 2 + S3) and works with save files. It starts on Sonic 1 + S3: fire,
  bubble and lightning shields from the monitors, and Sonic's insta shield on a second jump press. Time Attack keeps
  the classic shields.
- **The 7th Chaos Emerald:** a new Options setting, Max emeralds 6 / 7 (the 2013 release's hidden one), on by default
  and kept in save files. It adds the 7th special stage; with all seven emeralds Sonic can turn Super Sonic. The save
  select shows the 7th emerald.
- **Every character from the start:** Tails, Knuckles and Sonic & Tails no longer need unlocking.
- **No more freeze in the special stages:** a pause of more than half a second, when the background animation
  changed, is gone.
- **Faster special stages:** in emulators the rotating maze now plays at about 92 % of full speed, up from about 87 %.
- **Smoother zones:** Green Hill, Labyrinth and Star Light with Sonic & Tails run a little faster; Labyrinth with
  Sonic & Tails is now within a few percent of full speed.
- **Faster game scripts:** the engine now reads the game's script variables directly instead of looking each one up
  every time, which speeds up every stage a little.
- **More free memory** for the game.
- Apart from the new settings, nothing looks or plays differently: every change was checked frame by frame against
  the previous version.
