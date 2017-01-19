---
title: 0.1.14.6
---

#### Alpha release.
[https://github.com/Asnivor/MedLaunch/releases/tag/0.1.14.6](https://github.com/Asnivor/MedLaunch/releases/tag/0.1.14.6)

#### Notable Additions
* Added 32000Hz audio sample rate option
* Games library case-insensitive search
* Game path handling overhaul (fixed pce CD games not launching)
* Error handling and fixes to missing game or ROM folders (library games are marked as hidden until found again)
* Moved to semantic versioning
* Threaded game library import (so application doesnt appear to 'hang')
* Added context menu options in the games library for deleting all games in the database

#### Current Issues
* If upgrading you **MUST** either install MedLaunch in a new directory, or make sure to delete your existing MedLaunch.db database file before launching the new version. This will be fixed very soon.
* The launcher currently only handles absolute paths correctly. Relative path handling may or may not work but this part of the code needs a proper overhaul
* It is recommended that you use a brand new Mednafen instance for the time being. You can download the latest version of Mednafen from the Mednafen website. If you do not do this you might experience issues with already existing system specific configuration files in the Mednafen folder. Specifically, these will override base settings in MedLaunch until said system configuration is enabled in the launcher. This will be addressed in future releases.