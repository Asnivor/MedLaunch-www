---
title: 0.1.15.7
---

#### Alpha release.
[https://github.com/Asnivor/MedLaunch/releases/tag/0.1.15.7](https://github.com/Asnivor/MedLaunch/releases/tag/0.1.15.7)

#### Notable Additions
* Various bug-fixes
* Added system specific debug config controls
* Added WonderSwan specific config controls
* Added games library context menu option 'copy launch string to clipboard'
* Added a 'Set GUI Zoom' selector on the settings tab. Useful for people with tiny resolutions who cant see all content (and people with large resolutions who want the GUI content bigger)
* Added Mednafen directory selectors (cheats, snaps, sav etc)
* Added System BIOS/Rom path controls

#### Current Issues
* If upgrading you **MUST** either install MedLaunch in a new directory, or make sure to delete your existing MedLaunch.db database file before launching the new version. This will be fixed very soon.
* The launcher currently only handles absolute paths correctly. Relative path handling may or may not work but this part of the code needs a proper overhaul
* It is recommended that you use a brand new Mednafen instance for the time being. You can download the latest version of Mednafen from the Mednafen website. If you do not do this you might experience issues with already existing system specific configuration files in the Mednafen folder. Specifically, these will override base settings in MedLaunch until said system configuration is enabled in the launcher. This will be addressed in future releases.