# Home-Assistant Configuration
🏠 My Home-Assistant config and documentation.


Hey! Welcome to my home! It's powered by **Home-Assistant**.
In this file I will try and lay out my setup, so you can see the different parts.


# Components

I will attempt to break this file down in to the following sections:

- Servers
- Networking
- Hubs
- Sensors
- Lighting
- Media Players
- Voice Assistants
- Credits


## Servers

I have two main server computers for running the various services I use.

**Home-Assistant Host**
|                |                          |
|----------------|-------------------------------|
|*Hardware*|Intel NUC / i5 / 8GB RAM`            |
|*Operating System*          |Ubuntu Server 18.04 LTS|
|*Apps*          |Docker |  
|| HAP-NodeJS |


| Docker Containers |
|--|
| Home-Assistant (Hassio) |
| Heimdall |
| Duplicati |
| grocy |

| Hassio Add-Ons |  |
|--|--|
| Check Home Assistant configuration | | 
| Configurator | | 
| Duck DNS| | 
| ESPHome||
| FTP | | 
| IDE | | 
| MQTT Server & Web client | | 
| Node-RED| | 
| Pi-hole | | 
| Portainer |  |
| SSH & Web Terminal | | 
| Samba Share| | 
| UniFi Controller| | 
| Visual Studio Code| | 


**Mac mini**
|                |                          |
|----------------|-------------------------------|
|*Hardware*|Mac mini (Mid 2011) / i5 / 16GB RAM            |
|*Operating System*          |macOS High Sierra 10.13.6|
|*Apps*          |Plex Media Server
||  Sonarr |
||  Radarr |
||  SABnzbd |
||  iTunes |
||  Backblaze backup


## Networking

All your files are listed in the file explorer. You can switch from one to another by clicking a file in the list.

## Hubs

There are some IoT things where I have not been able to get away from using a third-party hub.  I am currently using:

 - Hive Heating (British Gas)
 - Link Plus (Lightwave)

## Sensors

-- **Xiaomi Mijia Temperature x4**
Connected via **Bluetooth** to an **ESP32**, which is flashed with **ESPHome**, to allow communication with **Home-Assistant**.

-- **Bruh Multi Sensors x4**
Connected via **WiFi**, running code developed by Ben from **BruhAutomation**, allowing communication of **Temperature, Humidity, Light-level** and **Motion** to **Home-Assistant** over **MQTT**.

-- **RF Door Sensors**
Cheap RF door hall-effect sensors from Ali-Express that connect to a **Sonoff RF Bridge** to provide communication with **Home-Assistant** via **MQTT**.

## Lighting

For full **PAF** (Partner Acceptance Factor) in my home, I like to replace light-switches, rather than using replacement bulbs and other solutions.  This means that if someone comes to visit, there are no awkward conversations needed for how to operate the lights!  In the UK, there are very few brands that offer drop-in replacement light switches for home-automation.  I have been using **[Lightwave](https://lightwaverf.com/)** products for a number of years, and subsequently some of my switches are their Generation 1 devices (which I control using an RFXTRX box) and some are Generation 2 (which pair directly to Apple HomeKit.)

For other lights such as lamps, I am using **Sonoff Basics**.  These are easily added to existing lamps by simply chopping into their cord.  I have flashed these devices using **[Tasmota](https://github.com/arendst/Sonoff-Tasmota)**, to allow me to control them from **Home-Assistant** over **MQTT**

I also have bunch of RGB LED strips.  Most of these are **WS2811/B** or **WS2812** and are connected to **NodeMCU** boards.  These are flashed using **[ESPHome](https://esphome.io/)**, which I am running as a **Hassio Add-On**.

I also have some wireless light switches, added to rooms where the light switches are in pretty badly thought-out places.  For this I am using **Sonoff RF wireless switches**.  These are battery powered and communicate over 433MHz RF.  These connect to a **Sonoff RF Bridge** which is flashed with **[Tasmota](https://github.com/arendst/Sonoff-Tasmota)**, so that it can send signals to **Home-Assistant** over **MQTT**.


## Media Players

 - Apple TVs (x4)
 - LG webOS TV
 - Playstation 4
 - Volumio on RaspberryPi

## Voice Assistants
- Apple HomePod (Siri)
- 2x iPhones (Siri) / 2x iPads
- 2x Apple Watches (Siri)
- 1x Amazon Echo (2nd Generation)
 - 2x Amazon Echo Dot (2nd Generation)
 - 1x Amazon Echo Dot (3rd Generation)

## Credits
| Credit | Link |
|--|--|
| Home-Assistant |  |
| Hassio | | 
| Home-Assistant Podcast| | 
| Bruh Automation | |
| ESP Home| | 
| Tasmota | | 
