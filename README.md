# Rock Band Blitz Plus
# Introduction

### Rock Band Blitz Plus is a quality of life mod based on [MiloHax](https://github.com/hmxmilohax) Rock Band Blitz Deluxe Project.

This guide contains full instructions on how to install Rock Band Blitz Plus for PlayStation 3 or Xbox 360.

# Table of Contents  
- [Features](#features)
  - [Quality of Life](#quality-of-life)
- [What You'll Need](#what-youll-need)
- [Downloads](#downloads)
- [How to Install](#how-to-install)
  - [Installing on RPCS3 (Recommended for PC)](#installing-on-rpcs3-recommended-for-pc)
  - [Installing on PS3](#installing-on-ps3)
  - [Installing on Xbox 360](#installing-on-xbox-360)
- [Repo Setup (Advanced)](#repo-setup-advanced)
- [Dependencies](#dependencies)

# Features

## Quality of Life
* Faster Boot Time
* Faster "Discovering DLC" at Boot
* Offline Powerups
* Fine Tune Calibration to 1MS
* Added Keys Parts to songs

# What You'll Need

### Playing Rock Band Blitz Plus requires these things:

- **A vanilla copy of Rock Band Blitz** for PS3 or Xbox 360 that you can extract onto your PC. The **USA** version is required for PS3 (`NPUB30749`)
- For Console: A **modded/hacked PS3 or Xbox 360** and a way to transfer files to it, we recommend using FTP
- For Emulator: A **mid-to-high-end PC** capable of running RPCS3

# Downloads

# How to Install
*NOTE: Rock Band Blitz Plus on PS3/RPCS3 installs differently compared to the other Deluxe projects.*
## Installing on [RPCS3](https://rpcs3.net/) (Recommended for PC)

* **Install your North American copy of Rock Band Blitz** through the emulator. The [**official RPCS3 site covers this nicely**](https://rpcs3.net/quickstart).
  * Remember, **you need to be running** ***NPUB30749***. RPCS3 will tell you this in the game selection GUI under the `Serial` column.

* Go to [Repo Setup (Advanced)](#repo-setup-advanced) and follow the steps to install the repo on your computer.

* In the **NPUB30749** game folder, copy the **`main_ps3.hdr`** and **`main_ps3_0.ark`** to the repo folder `_build/_rebuild/ps3/gen`. 

* In the **`windows_bats`**, run **`build_ps3`**.

* Copy the files & folders inside **`_build/ps3`** to your **NPUB30749** game folder.

***Rock Band Blitz Plus is now installed!***

**To update Rock Band Blitz Plus**, repeat the above steps. You can click the `Watch` button (All Activity) to be notified about any updates that occur.


## Installing on PS3

**NOTE: You WILL need a HACKED/MODDED (CFW or HFW/HEN) PS3 in order to play this mod on console. We hope this is clear.**

**NOTE: Rock Band Blitz Plus only works with** ***North American (`NPUB30749`)*** **copies of the game on PS3.**

**WIP - COMING SOON**

***Rock Band Blitz Plus is now installed!*** 

**To update Rock Band Blitz Plus**, repeat the above steps. You can click the `Watch` button (All Activity) to be notified about any updates that occur.

## Installing on Xbox 360

**NOTE: You WILL need a HACKED/MODDED (RGH or JTAG) Xbox 360 in order to play this mod on console. We hope this is clear.**

* **Install your vanilla copy of Rock Band Blitz** to your console's hard drive.
  * In case anything goes wrong, we recommend that you **rename `default.xex` to `default_vanilla.xex`**.

* **Disable updates** for Rock Band Blitz in Aurora. Rock Band Blitz Plus rolls `TU5` into its base installation.

* Download [**Rock Band Blitz Plus for Xbox 360**]. 
  * **Copy the contents of it to where your copy of Rock Band Blitz is installed** (we recommend using FTP to do so). Select `Yes` to overwrite the files.

* We also recommend **clearing your song cache**, as well as your **system cache**.
  * *To clear your **song cache**, navigate to `System Settings > Storage > Rock Band Blitz` and delete the song cache.*
  * *To clear your **system cache**, navigate to `System Settings > Storage` and press `Y` to clear the system cache.*

***Rock Band Blitz Plus is now installed!*** We highly recommend you check out [**Optional Upgrades**](#optional-upgrades) for songs and other cool stuff you can add to your game.

**To update Rock Band Blitz Plus**, [**re-download it**] and repeat the above steps. You can click the `Watch` button (All Activity) to be notified about any updates that occur.

# Repo Setup (Advanced)

### Installing Required Dependencies

* Install [**Git for Windows**](https://gitforwindows.org/), [**Dot Net 6.0 Runtime**](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime), and [**Python**](https://www.python.org/downloads/) (version 3.9 or later).
  * Install **Git** and **Dot Net 6.0 Runtime** with their default options, and ***select "Add python.exe to PATH"*** on the **Python** installer.

![Python PATH](dependencies/images/pythonpath.png)

* Open a **new command prompt** (press `Win+R`, type `cmd` and press Enter), type in `pip install gitpython`, and press enter. Close the command prompt when it's done installing.

### Initializing the Repo

* Press the Code button and then Download Zip
  * Make a new **empty** folder, **Extract the contents into this folder**

### ***The folder should look like this once it's done:***

![Repo Folder](dependencies/images/repofolder.png)

***The Rock Band Blitz Plus repo is now set up!*** 
# Dependencies

[Git for Windows](https://gitforwindows.org/) - CLI application to allow auto updating Plus repo files

[Dot Net 6.0 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/6.0/runtime) - Needed to run ArkHelper

[Python](https://www.python.org/downloads/) - For user script functionality (NOTE: 3.9 or newer is highly recommended!)

[Mackiloha](https://github.com/PikminGuts92/Mackiloha) - ArkHelper for building Plus - SuperFreq for building .bmp_xbox highway images

[swap_rb_art_bytes.py](https://github.com/PikminGuts92/re-notes/blob/master/scripts/swap_rb_art_bytes.py) - Python script for converting Xbox images to PS3

[dtab](https://github.com/mtolly/dtab) - For serializing `.dtb` script files
