# Newspace final project: Weather Balloon

&nbsp;
![](./pic/P1040569-1024x682.jpg)


$~~~~~~~~~~~$
# **Project Goal 🎯** 

Using two Raspberry Pi 3 computers linked by a TP-Link dongle, the project aims to build and implement a high-altitude weather balloon system. The main goal is to quickly ascend to an altitude of 30 km or higher and transmit a live video feed from the camera on the air station to the ground station. Using DJI VR technology, the live broadcast will be viewable on the ground station.



&nbsp;

-----
# **Summary**


Using two Raspberry Pi 3 computers connected by a TP-Link dongle, the project entails building a weather balloon system. The Raspberry Pi air station has a camera, while the Raspberry Pi ground station serves as the control panel. The air station's camera will record live video as the balloon quickly ascends to an altitude of 30 kilometers or higher.

To accomplish this, the ground station and air station will connect wirelessly via the TP-Link dongle. During the ascent, the camera on the air station Raspberry Pi will capture video footage, and the air station Raspberry Pi will transmit the live stream to the ground station in real time.

The live stream will be received and viewed on the ground station utilizing DJI VR technology. The user can watch the high-altitude environment from the perspective of the weather balloon in this unique viewing experience.

Aside from the live feed, the Raspberry Pi ground station will continue to gather and evaluate weather data supplied by the air station. This information, together with the live video feed, can be used for scientific research, weather analysis, and education.

In brief, the project's goal is to create a high-altitude weather balloon system out of Raspberry Pi machines linked via a TP-Link dongle. The apparatus will rapidly ascend to an height of 30 kilometers or higher and broadcast a live stream from the air station's camera. The live broadcast will be accessed on the ground station with DJI VR technology, providing an immersive picture of the high-altitude environment for research, analysis, and education.

$~~~~$

----
# Open sources being used


| Open-HD   |
|:----:|
|[![OpenHD](https://github.com/OpenHD/OpenHD/blob/2.3-evo/wiki-content/Open.HD%20Logo%20Splashscreen/Plain_OpenHD_Logo.jpg?raw=true)](https://github.com/OpenHD/OpenHD)|

&nbsp;
|  WFB-NG  |
|:----:|
|[![WFB-NG](https://github.com/svpcom/wfb-ng/blob/master/doc/logo-big.png?raw=true)](https://github.com/svpcom/wfb-ng)|

&nbsp;
| EZ-Wifibroadcast  |
|:----:|
|[![EZ-Wifibroadcast](https://raw.githubusercontent.com/richardbmx/EZ-WifiBroadcast/develop/logo115.png)](https://github.com/rodizio1/EZ-WifiBroadcast)|

 


&nbsp;

----
# Hardware



| Raspberry PI 3 x2 with camera| TPLink x2| DJI-VR
|:----:|:----:| :----:|
|![](./pic/Raspberry-Pi-3-with-camera-module.png)|![](./pic/giant_218539.jpg)| ![](./pic/dji-goggles-vr-brille-fast-neu.jpg)|

&nbsp;
##  Raspberry PI 3 description

![](./pic/Raspberry_Pi_3_Large.jpg)



------------------


&nbsp;
# LOG & Issues:


|                |What we have tried                         |Highest Reached distance                         |
|----------------|-------------------------------|-----------------------------|
|WFB-NG |1. Flashed the tool on two sd cards, one for air station and one for ground station. <br/> 2. Tried to achieve connection between two devices with no success via ssh and linux commands. <br/> 3. Reached out the community without any advancement.             | None           |
|OpenHD          |1. Flashed the tool on two sd cards, one for air station and one for ground station. <br/> 2. We managed to get a connection between the two PI's and started conduct experiments. <br/> 3. First experiment highest achieved distance was 20 meters because we were lack of hardware (extra battery, additional portable monitor). <br/> 4. We managed to get a DJI VR system and we have achieved a distance of 70 meters. <br/> 5. We did some terminal commands to improve the distance: Different channels, disabled the power management of the Network adapters & Changed the power so both adapters will get more power. Later we conducted another experiment and reached 100 Meters. <br/> 6. After doing a research on OpenHD using the aid of the Official Community in the Telegram & Forums & endless googling & ChatGPT we changed additional properties in the gui of the ground station (both devices had to be connected) The changes were: Manually increased the power level of the Adapters (the option appeared to be different than the one in the terminal), STBC turned on, Changed the frequency, In the hardware we changed the antennas of the Network adapters. Later on an experiment was conducted and we have reached a distance of 140 Meters. <br/> 7. An even higher distance was required but we did not manage to achieve it. Therefore, we have changed to another tool.               |140 Meters            |
|EZ-WifiBroadcast          |1. Flashed the tool on two sd cards, one for air station and one for ground station. <br/> 2. Tried conducting an experiment, we reached a distance of 240 meters (could be even longer).<br/> 3. Changed properties in the config files as suggested in the official github website. <br/> 4. Conducting another experiment, as soon as started devices are unable to communicate. <br/> 5. Flashed the sd card multiple times with different version (from newest to older versions). <br/> 6. Still no connection. |240 Meters|


















