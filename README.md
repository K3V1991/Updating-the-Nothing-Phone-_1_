<p align="center"><img src="https://github.com/K3V1991/Updating-the-Nothing-Phone-_1_/blob/main/Update-Nothing-Phone.png" width="200"></a>
<h1 align="center"><b>Updating the Nothing Phone (1)</b></h1>
<br />

<p align="center">
<a href="https://ko-fi.com/k3v1991" alt="Ko-fi"><img src="https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white"> &emsp;
<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=HW8B98TVDLKWA" alt="PayPal"><img src="https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white"> &emsp;
<a href="https://github.com/K3V1991/Donate-Crypto/blob/main/README.md" alt="Crypto"><img src="https://img.shields.io/badge/Bitcoin-000?style=for-the-badge&logo=bitcoin&logoColor=white">
</p>
<hr />
<br />

## Requirements:
* PC
* Platform Tools - [Android Developers](https://developer.android.com/studio/releases/platform-tools)
* Update File - reindex-ot.github.io - [GitHub](https://reindex-ot.github.io/) or Nothing Phone 1 update tracker - [XDA](https://www.xda-developers.com/nothing-phone-1-nothing-os-update-tracker/)
<br />
<br />

## Install via Recovery:
Sideload the Update Packages through the Recovery Interface

1. Download the Update Zip File on your PC
2. Make sure the Nothing Phone (1) is discoverable by ADB from your Computer
3. On your Computer, enter the following Command:
```
adb reboot recovery
```
4. The Phone reboots, you should see "No command" on the Screen. 
5. Now press and hold the Power Button of your Phone. While you hold Power, press the Volume Up Button and let go of both Buttons quickly. You should the Android Recovery Menu.
6. On your Phone, select the "Apply update from ADB" Option.
7. Run the Command: 
```
adb devices
```
8. This should return a Device Serial with the "sideload" next to its Name, indicating that your Device is connected to the Computer in Sideload Mode.
9. On your Computer, type:
```
adb sideload "filename".zip
```
(Replace "filename" with the full Path, followed by the Name of the File. <br />
11. The Update should install on your Phone. Once the Installation is complete, choose "Reboot system now" to reboot into the new Build.
<br />
<br />

## Install via Local System Update:
Built-in System Update Installation App

1. Create a Folder named "ota" at the Root of the Internal Storage of your Phone. Copy the Update Zip File to that Folder.
2. Dial ```*#*#682#*#*``` to open up the Offline Update Tool.
Note: You can also use an Activity Launcher App to execute the "OfflineOTAUpgrade" Tool. The Package Name is "com.nothing.OfflineOTAUpgradeApp".
3. The Wizard will try to locate any valid OTA File present in the Internal Storage and install it. In case it fails, manually browse for the OTA Package.
4. After selecting the OTA File, the Wizard will apply the Update and reboot the Device.
<br />

## Verification:
A simple Way to check if you have followed all of these steps correctly and sideload the OTA File properly is to head to Settings > About phone > Software info. <br />
This should be on the exact Nothing OS Version that you have sideloaded, indicating that you’ve successfully managed to complete the Installation Process.
