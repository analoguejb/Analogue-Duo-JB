# Analogue Duo
### Instructions
- Extract everything to the root of your SD card and be sure to first remove any existing firmware file
- Everything else goes into /Assets/pce/common/
- CD files must be in their own individual subfolder with the respective cue/bin inside and it is recommended to organize other files in subfolders 
- Optionally, place a System Card BIOS (with extension .pce) inside /Assets/pce/common/BIOS/
###  JB Firmware V0.9
- You can enable "Resume Browser" in the options so the browser will remember the last game selected
- You can disable "Auto-add to Library" to prevent every game you start from being added to the Library
- For original System Card functionality a .pce placed in the BIOS folder will override Duo's own built-in BIOS, for example, playing audio and CD+G discs
- When loading a subfolder Duo checks if there is exactly 1 .cue file inside. If so, it will be treated as a CD game
- BIOS preferences can be adjusted per CD game. If there is exactly 1 .pce BIOS file inside a CD subfolder, that BIOS will automatically replace the default BIOS when running that game
- A physical System Card will take precedence over all other specified BIOS
- WAV files are supported for audio tracks. WAV files must have a standard 44 byte header and contain an exact multiple of 2352 bytes (1 frame of CD audio), not accounting for the header
- CD+G discs are supported. The track type should be "CDG" in the .cue, with a sector size of 2448 bytes
- You can force SuperGrafx mode by naming the file with the extension ".sgx"
- CD Backup RAM, which sometimes can be utilized by specific Hucards, is recognized by game signature
