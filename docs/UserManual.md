---
layout: default
title: SteamAutoCrack User Manual
description: SteamAutoCrack User Manual
---

<a href="/docs/" class="btn btn-primary">Back to docs index</a>

# User Manual

## Main Options

### Path

* Set the Steam clean game file folder (Make sure to choose the root game path, for example in UE4 games you should choose the folder that includes the `Engine` folder), game executable or steam_api(64).dll.

### Start Crack

* Start the crack process.
* The `Delete Previous steam_settings Folder` is the same as `Goldberg Steam Emulator Configuration`'s.

***

## 1. Generate Goldberg Steam Emulator Game Info

### Steam App ID

* Set the Steam App ID.
* App ID can be found using the built-in `App ID Finder` or [SteamDB](https://steamdb.info/).

### Generator API

* Generate game info with different info APIs.
* SteamKit2 Client: Use SteamKit2 Client for generating most of the info and Steam Web API API for game schema. (Best result)
* Steam Web API: Steam Web API API for all game info. (Faster but less info)
* Offline: Generate offline basic info without Internet.

### Steam Web API Key / Steam Web API Access Token

* Your Steam Web API Key or Steam Web API Access Token.
* You have to choose one of them to generate game info completely
* Get a Steam Web API Key require a Steam account with 5$ spent on Steam, but you can get a Steam Web API Access Token without it.
* You can get your Steam Web API Key from [Steam Web API Key](https://steamcommunity.com/dev/apikey).
* You can get your Steam Web API Access Token for following steps:
  1. Login into [Steam](https://store.steampowered.com) in your browser.
  2. Access [https://store.steampowered.com/pointssummary/ajaxgetasyncconfig](https://store.steampowered.com/pointssummary/ajaxgetasyncconfig) on your browser.
  3. Response will like this `{"success":1,"data":{"webapi_token":"eyAidHlxxxxx"}}`, the value of `webapi_token` is your Steam Web API Access Token (The `eyAidHlxxxxx` field).

### Use Steam Web App List

* Use Steam Web App List for faster game info generating.

### Generate Achievement Images

* Generate game achievement images (icons) for Goldberg Steam emulator. (Now it's much faster)

***

## 2. Generate Goldberg Steam Emulator Configuration

### Language

* Set the language the emulator will report to the game.
* Default language settings will be generated from your system language.

### Listen Port

* Set the UDP/TCP port the emulator listens on (You should probably not change this because everyone needs to use the same port or you won't find yourselves on the network).

### Account Name

* Set your name in game.

### Steam ID

* Set your emulator steam id.
* If your saves for a game are locked to a specific steam id you need to change this value.

### Disable Networking

* Disable all the networking functionality of the Steam emulator.

### Offline mode

* Enable Steam emulator Offline mode.
* Some games that connect to online servers might only work if the Steam emulator behaves like steam is in offline mode.

### Enable Overlay

* Enable the Steam emulator overlay.
* This is for games that depend on the steam overlay to let people join multiplayer games.
* Use SHIFT-TAB to open the overlay.

### Custom Broadcast IP

* Set custom IPs (or domains) which the emulator will send broadcast packets to.

### Ticket

* Set the Encrypted App Ticket for the game.

### Open Example Config

* Open Goldberg Emulator Example Folder.

### Open Config Folder

* Open Goldberg Emulator `steam_settings` folder in Temp file.

***

## 3. Unpack SteamStub

* Requires selecting .exe File or Folder as input path.

### Keep Bind Section

* Keep .bind Section after unpack, required if unpacked executable won't run.

### Use Experimental Features

* Required if unpacked executable won't run.

### Realign Sections

* Realign executable sections.

### Keep DOS Stub Data

* Keep executable DOS Stub Data.

### Recalculate File Checksum

* Recalculate Executable Checksum.

### SteamAPICheckBypass Mode

* Use [SteamAPICheckBypass](https://github.com/oureveryday/Steam-API-Check-Bypass) to bypass steam_api(64).dll and exe integrity check.
* Disabled: Disable Apply SteamAPICheckBypass.
* SteamAPICheckBypass DLL: DLL Name for DLL hijacking to game executable.
* Enable All Time: Intercept All steam_api(64).dll read requests and all game exe read requests.
* Enable Only Nth Time: Intercept steam_api(64).dll read request only on Nth time and all game exe read requests.
* Enable Only Not Nth Time: Intercept steam_api(64).dll read request only not on Nth time and all game exe read requests.
* `Enable Only Nth Time` and `Enable Only Not Nth Time` are useful for custom requirements.
* SteamAPICheckBypass won't intercept `LoadLibrary` now.

***

## 4. Apply Goldberg Steam Emulator

* Requires selecting steam_api(64).dll File or Folder as input path.

### Use Custom Save Location

* Default save path: `C:\Users\<Your windows user name>\AppData\Roaming\Goldberg SteamEmu Saves\<appid>\settings`
* Create a `local_save.txt` beside steam_api(64).dll to change default Goldberg emulator game save path.

### Use Experimental version Goldberg Emulator

* Uses Experimental version of Goldberg Emulator.

### Generate Steam Interfaces file

* Automatically Generate steam_interfaces.txt if the original steam_api(64).dll is older than May 2016 (Determined with Digital Signature Timestamp).

### Force Generate for each steam_api(64).dll

* Generate steam_interfaces.txt for each steam_api(64).dll.

***

## 5. Generate Crack Only Files

* Requires selecting Folder as input path.
* Crack only files will be generated in the `Crack` folder.

### Output Path

* Set the place to put crack only files.

### Create Crack Readme File

* Create Crack_Readme.txt which includes info on how to apply the crack only files.

### Pack Crack Files with .zip archive

* Pack Crack Files into a Crack.zip archive.

***

## 6. Restore Crack

* Requires selecting Folder as input path.
* Restores Crack Generated with SteamAutoCrack.

***

## AppID Finder

### Fuzzy Search

* If fuzzy search is disabled, will use exact search.

***

## Settings

### Save Config File

* Save Config.json with SteamAutoCrack options.

### Enable Debug Log

* Enable Debug Log Level.

### Output Log to File

* Output all Logs to log.log file.
* Error logs will always output to error.log regardless of whether this option is disabled.

### Update/Download

* Update or download latest version of Goldberg Steam Emulator if it does not exist or an update is available.

### Force Update Steam App List

* Update Steam App List now.
* Steam App List will automatically be updated daily.