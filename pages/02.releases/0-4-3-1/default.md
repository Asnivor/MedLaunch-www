---
title: 0.4.3.1
---

[https://github.com/Asnivor/MedLaunch/releases/tag/0.4.3.1](https://github.com/Asnivor/MedLaunch/releases/tag/0.4.3.1)

#### Important Release Notes
** This MedLaunch release is *ONLY* compatible with version 0.9.42.x of Mednafen. Do *NOT* upgrade if you are not planning to update Mednafen also **

**_This is primarily a bugfix release._**

**_If you are seeing MedLaunch crash whilst opening please either:_**

* **_Extract this version of MedLaunch to a new folder and run it_**

**_or_**

* **_Extract this version over your current MedLaunch folder, then delete MedLaunch.db from MedlaunchDIR\Data\Settings before running the application_**

Otherwise follow the usual instructions below.

#### Notable Additions
* (Bugfix) Fixed exception(crash) caused by mednafen application not being properly initialised before importing configs into MedLaunch
* (Bugfix) Added null-check on netplay servers datagrid (mitigates application exception if the database didnt initialise correctly with the pre-defined servers)
* (Bugfix) Fixed localisation lookup issue when attempting to determine the mednafen version from the mednafen output log (stdout.txt)
* (Addition) Added another public netplay server to the list

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.42.x branch - 64-bit version is required if you want to emulate Saturn games). 
* You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
* If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade
##### Preferred Method: 
* Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
* Ensure you have the correct version of Mednafen installed (v0.9.42.x)
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else

##### Manual Method: 
* You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
* Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else