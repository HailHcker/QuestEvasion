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
<br />

**ADB:**
```
DISABLE:
adb shell pm disable com.oculus.unifiedtelemetry
adb shell pm disable com.oculus.gatekeeperservice
adb shell pm disable com.oculus.notification_proxy
adb shell pm disable com.oculus.bugreporter
adb shell pm disable com.oculus.os.logcollector
adb shell pm disable com.oculus.appsafety

ENABLE:
adb shell pm enable com.oculus.unifiedtelemetry
adb shell pm enable com.oculus.gatekeeperservice
adb shell pm enable com.oculus.notification_proxy
adb shell pm enable com.oculus.bugreporter
adb shell pm enable com.oculus.os.logcollector
adb shell pm enable com.oculus.appsafety
```

## Disable Updates
**Disable:**
<br />

```
adb shell pm disable --user 0 com.oculus.updater
```
<br />

**Enable:**
```
adb shell pm enable --user 0 com.oculus.updater
```

## Ban Evading
**Not Tested Will Be Updated As We Go**
1. Sideload AndroidIDeditorV2 and follow the instructions to spoof
<br />
Note: you might need to use a vpn

## HZ
**Sidequest:**
1. Click the crow bar at the top left
2. Select hz
<br />

**ADB:**
```
adb shell settings put system vr_mode_refresh_rate <HZ>
adb reboot

LOWER THEN 60HZ:
adb shell setprop debug.oculus.swapInterval 4
```

## Modding
There are many ways to mod on quest, but the two main ones are:
1. Quest Patcher
2. Lemon Loader
<br />

**Quest Patcher:**
There are not very many resources, and the ones that exist are pretty [bad](https://github.com/Lauriethefish). But The [BeatSaber modding group](https://discord.com/invite/beatsabermods) is about as good as your going to get.
<br />

**Lemon Loader:**
Lemon Loader is a lot better in my opinon, as its just easier to use. There are many videos of [how to install lemon loader](https://www.youtube.com/watch?v=v2BhWfnzwm4), there are also many resources to [make mods](https://mod.io/g/bonelab/r/lemon-loader-mods-quest-code-mods)

# Theory For Bypassing Oculus (NOT TESTED)
1. Sideload Oculess
2. Disable Oculus Companion Server
3. Disable Updates ```adb shell pm disable --user 0 com.oculus.updater```
<br />

since this locks all oculus features including the library, in theory you can use ADB commands to open any app. And any app that **doesnt** use Oculus API can be played just fine IN THEORY.

4. Get the application you want to run ```adb shell list packages```
5. Run the application ```adb shell am start -n com.package.name/.ActivityName```
<br />

To install new games you could use something like [OculusDB](https://oculusdb.rui2015.me/) to get the APK, then sideload it.

# Resources
#### Evasion:
https://github.com/basti564/Oculess
#### Spoofers
https://github.com/sdex/AndroidIDeditorV2
#### Sideloading
https://sidequestvr.com <br />
https://wiki.vrpirates.club/ <br />
https://oculusdb.rui2015.me/
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

#### Downgrading
https://github.com/basti564/DownQuest

#### Modding
https://github.com/LemonLoader/MelonLoader <br />
https://www.youtube.com/watch?v=v2BhWfnzwm4 <br />
https://mod.io/g/bonelab/r/lemon-loader-mods-quest-code-mods <br /> <br />

https://github.com/Lauriethefish/QuestPatcher <br />
https://github.com/danrouse/beatsaber-quest-modding-guide <br />
https://discord.com/invite/beatsabermods

# Credits
Big thanks to [@basti564](https://github.com/basti564) alot of this github is a compiled source from them.
