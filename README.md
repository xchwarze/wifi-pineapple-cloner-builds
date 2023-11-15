# Wifi Pineapple Cloner: Builds

For a long time I have noticed that there are people stealing the authorship of this project that started in 2018.<br>
Also there is people who go further and are selling the devices ready to use...<br>

So to prevent anyone from being scammed paying for something that is public and free, I decided to make a second repo with the builds already generated.


## Issues and Pull Request

All this will be handled in the [original project](https://github.com/xchwarze/wifi-pineapple-cloner).


## Supported devices

All builds are made with:
* OpenWrt 19.07.7
* Wifi Pineapple Cloner (WPC) v4
* The config used to build was the "universal" (flavor: universal).<br>
This is designed to be able to mount a TETRA on any hardware.
<br>

The process will work correctly only if you follow these steps:
* First install OpenWrt 19.07.7 on the device.
* Then install the update you will find in this repository.<br>
You must install it with the `do not save configuration over reflash` option checked.
* Your hardware has to have at least 2 wifis and it would be recommended to have 3.<br>
To comply with this you can use the usb adapters mentioned in the `Recommended setup`.
* Your hardware must have a pendrive or sd card in order to have the available space needed by the pineapple.<br>
It has to be formatted using the tool provided by the panel under `Advanced > USB & Storage > Format SD Card`.
* As tetra is made to be used on hardware with 32 MB of flash I had to cut some dependencies from the default installation.<br>
These dependencies will be installed automatically when the pinapple is connected to the internet and booting.<br>
If you want to manually run this process `wpc-tools missing_packages`<br>
Without these dependencies you will not be able to use the live scan type and some modules. However you will be able to use the timed scans and the rest of the tools.
* The default ssh password is `root`. This will be useful when debugging problems that may occur during installation.
<br>


### Attention!

This repo moved to Gitlab