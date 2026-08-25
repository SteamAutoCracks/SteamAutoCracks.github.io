---
layout: default
title: SteamAutoCrack FAQ
description: Frequently Asked Questions
---

<a href="/docs/" class="btn btn-primary">Back to docs index</a>

# General FAQ  

> * **Q1: How do I use this tool to crack a game/app?**  
> * **A1:** You need clean Steam game/app files and an internet connection (optional) to proceed with cracking.  

> * **Q2: What kind of DRM can this tool crack?**  
> * **A2:** This tool only works with games/apps that have a standard Steam API check and SteamStub DRM. It **won't work** on other DRM protections like Denuvo, VMProtect, etc.  

> * **Q3: What games/apps are compatible with this tool?**  
> * **A3:** This tool works with games/apps that are not online-only. The game must have a normal Steam API check and SteamStub DRM. It successfully cracks up to 95% of Steam offline games/apps.  

> * **Q4: Does this tool work for online games?**  
> * **A4:** This tool works with only a few online games. In most cases, it **won't work** for online titles.  

> * **Q5: The tool is detected as a virus.**  
> * **A5:** This tool **is not** a virus. The entire source code is open and available for review. The latest 3.0 version should have resolved this issue. You can verify it via [VirusTotal](https://www.virustotal.com/gui/file/366c1861aa7631194e026a0a6f2a0d1d002a440debb5e0cf4ba7f98b3dd5bbb0).  

> * **Q6: How to get a Steam Web API Access Token?**  
> * **A6:** 1. Login into [Steam](https://store.steampowered.com) in your browser.
>  2. Access [https://store.steampowered.com/pointssummary/ajaxgetasyncconfig](https://store.steampowered.com/pointssummary/ajaxgetasyncconfig) on your browser.
>  3. Response will like this `{"success":1,"data":{"webapi_token":"eyAidHlxxxxx"}}`, the value of `webapi_token` is your Steam Web API Access Token (The `eyAidHlxxxxx` field).
---

# Troubleshooting  

> * **Q1: I encountered an error while cracking!**  
> * **A1:** Please report the error in the [GitHub Issues section](https://github.com/SteamAutoCracks/Steam-auto-crack/issues).  

> * **Q2: The program won't start.**  
> * **A2:** Please try downloading and installing the [.NET 8.0 **Desktop** Runtime](https://dotnet.microsoft.com/download/dotnet/8.0/runtime). If the issue persists, report it in the [GitHub Issues section](https://github.com/SteamAutoCracks/Steam-auto-crack/issues).  

> * **Q3: I received the error `Insufficient privileges to get access token for app (AppID)` while cracking.**  
> * **A3:** If the AppID is the game's main AppID, the crack process was not completed. Please **Restore Crack** first, then change **Generator API** to **Steam Web API**, and try again.

> * **Q4: I cannot use the `AppID Finder` or cannot find latest game while cracking.**  
> * **A4:** Please fill your Steam Web API Key or Steam Web API Access Token, then open `Settings` and click `Force Update Steam App List`.

> * **Q5: Unable to get the achievement data for Goldberg Emulator.**  
> * **A5:** Please fill your Steam Web API Key or Steam Web API Access Token.
