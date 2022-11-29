---
description: Setting up Hideez USB Bluetooth Dongle on Linux
---

# How to use Hideez Bluetooth Dongle on Linux

## Ubuntu

{% hint style="info" %}
Click [here](https://help.ubuntu.com/lts/ubuntu-help/bluetooth.html) for official documentation on how to use Bluetooth.
{% endhint %}

{% hint style="warning" %}
**Please, note:** If your laptop has a built-in Bluetooth adapter, [it will need to be disabled ](https://projectgus.com/2014/09/blacklisting-a-single-usb-device-from-linux/)before using the USB Bluetooth adapter. Don’t uninstall the Bluetooth management software in the last step!
{% endhint %}

For other Linux distributions, you’ll need to install the BlueZ Bluetooth stack and the BlueMan Bluetooth Manager. Consult your distribution’s website to see if the Bluez and Blueman software are available as a ready-to-install software package.

#### **Turning on Bluetooth**

1. Plug in the Bluetooth adapter
2. Click the Bluetooth Icon in the toolbar
3. Click turn on Bluetooth

#### **Connecting a Device**

1. Click the Bluetooth icon in the menu bar and select Set Up New Device.
2. Make the other Bluetooth device [discoverable or visible](https://help.ubuntu.com/lts/ubuntu-help/bluetooth-visibility.html) and place it within 20 meters (about 65 feet) of your computer. Click Continue. Your computer will begin searching for devices.
3. If there are too many devices listed, use the Device type drop-down to display only a single type of device in the list.
4. Click the PIN option to set how a PIN will be delivered to the other device.
5. The automatic PIN setting will use a six-digit numerical code. A device with no input keys or screen, such as a mouse or headset, may require a specific PIN such as 0000, or no PIN at all. Check your device’s manual for the proper setting.
6. Choose an appropriate PIN setting for your device, then click Close.
7. Click Continue to proceed. If you did not choose a preset PIN, the PIN will be displayed on the screen.
8. If required, confirm the PIN on your other device. The device should show you the PIN you see on your computer screen or may prompt you to enter the PIN. Confirm the PIN on the device, then click Matches.\
   \
   You need to finish your entry within about 20 seconds on most devices, or the connection will not be completed. If that happens, return to the device list and start again.\

9. A message appears when the connection successfully completes. Click Close.

#### **Set Playback Devices**

1. Click the Speaker icon on the toolbar and select Audio Setup
2. Select the Audio Hardware Setup Tab
3. Click the Profile drop-down box and select Off

## KDE and GNOME

The KDE and GNOME desktop environments provide Bluetooth configuration and management utilities. If not installed by default, you will need to install them with your Linux distribution’s package manager.

Debian, Linux, Ubuntu, and Ubuntu derivatives usually have the Bluez Bluetooth stack installed by default along with a Bluetooth manager. We recommend opening a terminal window and typing the following command to install the necessary packages:

```
sudo apt-get install bluez blueman
```

If the packages are already installed, apt-get will report that the packages are already present on your system.

Then follow the steps [described above](how-to-use-hideez-bluetooth-dongle-on-linux.md#turning-on-bluetooth).
