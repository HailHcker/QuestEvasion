# YOU WILL NEED DEVELOPER MODE
https://www.youtube.com/watch?v=jB1gwgSpU3E

## Listening To Music
1. Sideload Spotify
2. Sideload Oculess
3. Open Oculess
4. Click the "Background Audio For All" button
5. Load Spotify
<br />
Note: You will have to do this everytime after a restart

## Disable Oculus Servers
1. Sideload Oculess
2. Open Oculess
3. Click the "Disable Oculus Companion Server" button

## Enable/Disable Telementary Apps
1. Sideload Oculess
2. Open Oculess
3. Click the "Disable/Enable Telementary Apps" button

## Ban Evading
1. Disconnect from wifi on quest
2. Sideload AndroidIDeditorV2 and follow the instructions to spoof
3. Make a new oculus account
4. Connect Back to wifi
<br />
Note: you might need to use a vpn

## HZ
**Sidequest:**
1. Click the crow bar at the top left
2. Select hurts 
<br />
**ADB:**
<br />
```
adb shell settings put system vr_mode_refresh_rate <HZ>
adb reboot

LOWER THEN 60HZ:
adb shell setprop debug.oculus.swapInterval 4
```

# Resources
#### Evasion:
https://github.com/basti564/Oculess
#### Spoofers
https://github.com/sdex/AndroidIDeditorV2
#### Sideloading
https://sidequestvr.com <br />
https://wiki.vrpirates.club/
```
adb install file.apk
```
#### ADB
###### WINDOWS
```
install ADB:
https://dl.google.com/android/repository/platform-tools-latest-windows.zip

CD <DIR>

adb devices //Check if your oculus is connected
adb connect <YOUR LOCAL IP>
```
###### LINUX
```
sudo apt-get install android-tools-adb
adb devices //Check if your oculus is connected
adb connect <YOUR LOCAL IP>
```
###### MAC
```
brew install android-platform-tools
adb devices //Check if your oculus is connected
adb connect <YOUR LOCAL IP>
```
#### Music
https://m.apkpure.com/spotify-music-i/com.spotify.music
