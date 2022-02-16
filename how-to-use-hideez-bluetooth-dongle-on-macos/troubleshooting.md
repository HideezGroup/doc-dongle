---
description: Hideez USB Bluetooth Dongle - Troubleshooting for macOS
---

# Troubleshooting

1\. Delete all paired devices in the list of bluetooth devices.\
2\. Insert the dongle into the USB port.\
3\. Make sure that the dongle is working - it should be blinking blue when Bluetooth is used.

{% hint style="warning" %}
Please, notice: Dongle may shortly blink once when it plugged into the USB port. It may not be blinking while Bluetooth is not used!
{% endhint %}

4\. Write the following command in the terminal: **sudo nvram bluetoothHostControllerSwitchBehavior = always** \
5\. Restart your PC. \
6\. Pull out and insert the dongle back. \
7\. In the bluetooth settings, check that Broadcom has changed to Cambridge Silicon. \
8\. Open the list of Bluetooth devices. Select the device you want to connect. Click the Connect button.&#x20;

### If your Bluetooth device does not connect:

1\) Make sure you have the latest OS version. \
2\) Connect another device. \
3\) Try the dongle on another PC. \
4\) If there are many Wi-Fi points nearby, then they will interfere with the functioning of Bluetooth. \
5\) If you are using a usb hub and the dongle does not work, try connecting it directly to your PC.

### Option for macOS Monterey:

1. Open Terminal command on your Mac and type following command **sudo pkill bluetoothd** and hit the **Return** to run.
2. Enter your Mac login password, wait for 5 seconds, and start using Bluetooth and set up the Bluetooth device.



### If none of the options above give the desired result, then try:

#### **Resetting Bluetooth**

Before you begin, you will need to close all applications.

1. Hold **Shift + Option** and select the Bluetooth icon on the menu bar
2. Select **Reset Bluetooth Module**
3. Reboot the system

Check the operation of Bluetooth; everything should work. Please, be aware that all devices will need to be re-configured.

Option for MacOS Monterey:

1. Open Terminal command on your Mac and type following command  **sudo pkill bluetoothd** and hit the **Return** to run.
2. Enter your Mac login password, wait for 5 seconds, and start using Bluetooth and set up the Bluetooth device.

#### **Deleting Bluetooth Settings File**

1. Launch **Finder**
2. Clamp the keyboard shortcut **Command + Shift + G**
3. In the window, specify the following path: **/ Library / Preferences/**
4. Find the Bluetooth settings files. They can be called "**com.apple.Bluetooth.plist**" or "**com.apple.Bluetooth.plist.lockfile**", delete them
5. Reboot, re-configure pairing with the necessary devices

In most cases, the first two methods are enough. However, if the problem still occurs, then we can try the third method.

#### **Resetting System Management Controller (SMC)**

1. Turn off your Mac
2. Hold the **Shift-Control-Option** keys simultaneously with the **power button** for 10 seconds and release
3. Turn on your Mac

SMC reset, it remains to check for Bluetooth.

You can also read more in [Apple's support article](https://support.apple.com/en-us/HT201171).

### **Still having trouble connecting your adapter?**

Here are a couple of useful tips that will help you fix some of the most common Bluetooth pairing issues:

* **Remove Old Bluetooth Connections -** If you’ve previously connected the dongle to a different device, you might experience issues with it trying to connect to the old connection instead of the new one. If you’re having such trouble, it’s best to reset your device and start fresh with the new connection.
* **Power Off and Back On -** The old and proven method of simply performing a soft reset can often do the trick. This is even simpler if you’re setting up Bluetooth on your mobile device, as you don’t even need to turn it off. Just go in and out of airplane mode.
* **Get Away from Your Wi-Fi -** Since Wi-Fi and Bluetooth operate in a relatively close spectrum, you might experience interference if you’re trying to connect to Bluetooth while near a Wi-Fi device. Move away from your router, and you might find that your Bluetooth will start working.
* **Charge Up The Device -** Modern computers and laptops have a smart power management function to preserve themselves when their battery is running low. They automatically turn off any functions that drain the battery too much, including Bluetooth. For this reason, you should always make sure that your device has enough juice before pairing it up.
* **Update Your Device’s Firmware -** If you can’t connect to your PC or Mac, consider that the issue could be coming from the device itself. Check if you have the latest firmware and update it to pair up with the dongle.

If you have any questions about these instructions or using Hideez Dongle, please contact our Customer Care team at support@hideez.com. We’ll be happy to help!
