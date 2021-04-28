# Downpatching guide

1) Download & Extract [Depot Downloader](https://github.com/SteamRE/DepotDownloader/releases/tag/DepotDownloader_2.4.0)
2) Create a batch file in the newly created folder with the following contents:
```bat
@echo off
Title Ghostrunner Downpatcher (v0.32091.481)
SET /P _username= Steam Username: 
call dotnet .\DepotDownloader.dll -app 1139900 -depot 1139901 -manifest 1667486716279452529 -username "%_username%" -remember-password -dir ".\Ghostrunner" -max-servers 30 -max-downloads 10
rmdir ".\Ghostrunner\.DepotDownloader" /s /q
echo 1139900 >> .\Ghostrunner\steam_appid.txt
pause
```
3) Run the batch file, enter your Steam credentials and wait for "Press any key to continue..." to appear in the console, it should take some time.
(If it fails or gets connection lost, ignore until the end and run it multiple times)

4) Once done go to your Steam Library, click 'Add a Game' (bottom left), 'Add a Non-Steam game', Browse and pick the `Ghostrunner.exe` within the created `Ghostrunner` folder and click 'Add Selected Programs'.

5) In Library, you can right click it -> properties and rename it, like.. "Ghostrunner - WinterPatch'.

---
Credit to [Dmgvol](https://github.com/Dmgvol) for writing the guide.