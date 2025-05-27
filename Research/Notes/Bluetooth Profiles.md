[[Bluetooth]], [[Driver]]

As previously stated, Bluetooth is like wireless USB. While it isn't 'plug,' we do want plug-n-play ease. 

# Issue of Drivers
Plug-n-play falls apart if the end user needs to install specific drivers on every device they want to use.

**The solution is generic/standardized drivers**
	Called Bluetooth profiles

# What is a profile
A profile is a standardized data transmission protocol using Bluetooth hardware coordinated by software optimized for a specific type of data transmission.
- The [Headset Profile (HSP)](https://en.wikipedia.org/wiki/List_of_Bluetooth_profiles#Headset_Profile_\(HSP\) "List of Bluetooth profiles") connects headphones and earbuds to a cell phone or laptop.
- The [Health Device Profile (HDP)](https://en.wikipedia.org/wiki/List_of_Bluetooth_profiles#Health_Device_Profile_\(HDP\) "List of Bluetooth profiles") can connect a cell phone to a digital thermometer or heart rate detector.
- The [Video Distribution Profile (VDP)](https://en.wikipedia.org/wiki/List_of_Bluetooth_profiles#Video_Distribution_Profile_\(VDP\) "List of Bluetooth profiles") sends a video stream from a video camera to a TV screen or a recording device.
- Advanced Audio Distribution Profile (A2DP) for most audio sharing
- Audio/Video Remote Control Profile (AVRCP) for audio/video
- Many more

Whatever Bluetooth driver an operating system uses to control a Bluetooth chip will contain several generic profiles.
# Proprietary Profiles
Since companies suck, a lot of devices such as airpods, and Ipods have proprietary profiles only available for certain operating systems.
	This means you can't use these Bluetooth devices without installing specific drivers, which may not be possible.

Rarely, Bluetooth devices such as RGB keyboards that have proprietary RGB keyboard profiles may still work with another generic profile with reduced features.