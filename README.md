# Home Assistant Config

Hey! This is my Home Assistant configuration. Under the screenshot of the front-end below you'll find the devices I'm using, the automations I have running, as well as some video examples. You can also browse through my configuration files above to see how I'm doing everything.

I am very regularly adding new devices, automations, and configurations. I'll keep this readme updated with the latest.

![Home Assistant front-end](http://i.imgur.com/buFzIfi.png)

# Devices

Here's the stuff I use to control my home. It's a mixture of Z Wave and Wifi devices, all controlled by Home Assistant and the Amazon Echo for voice, plus some other misc things thrown in the mix. What's great about having Home Assistant at the center of everything is you can mix and match devices and it treats them all the same. This keeps me from being locked to any one smart home vendor. Great job!

## Controller
* Raspberry Pi 3 running Home Assistant
* Aeotec ZW090 Z Stick (to interface with Z Wave network)

## Switches and lights
* GE Z-Wave Smart Dimmer Toggle Switch 12729 (x7)
* GE Z-Wave Smart Toggle Switch, On/Off 12727 (x3)
* Phillips Hue Bloom (x2)
* Phillips Hue White A19 (x2) with bridge
* WeMo Switch Smart Plug, Wi-Fi
* YEELIGHT Smart LED Bulb, Wi-Fi,60W Equivalent E26

## Voice control
* Amazon Echo
* Amazon Echo dot

## Presence detection
* Google Nexus 5X (2)
* Owntracks via MQTT (CloudMQTT)

## Misc
* Ecobee3 smart thermostat + sensors
* Simplisafe wireless home security system
* LiftMaster CIGBU Internet Gateway for MyQ garage door

# Automations

## Lights

* Turn on outside lights at sunset
  - If cloud cover is over 75%, turn them on 2.5 hours before sunset (because it's darker)
  - If cloud cover is under 75%, turn them on only 30 minutes before sunset (because it's brighter)
* Turn on morning light scene at sunrise
* Turn all lights off when wife and kids leave for school
* Turn on evening light scene at 4:30 PM every day
* Turn off all lights at midnight
* Turn on and off lights (independently or as a group) using Alexa [[video example]](https://youtu.be/am7hBSraAyA)

## Security
* Disarm the alarm every morning at 6:45 AM, turn on morning light scene
* When alarm is manually armed at night, turn on nighttime light scene [[video example]](https://youtu.be/EiiTg5AtEew)
* If alarm siren is activated, flash all controlled lights in house once per second until disarmed [[video example]](https://youtu.be/K4GNwNoDph4)
* Send mobile alert when garage door opens

## Media

* When Apple TV is playing (after 7pm), trigger media-playing light scene; when Apple TV is paused, trigger media-paused light scene [[video example]](https://youtu.be/wfzKJfB-_QY)

# Coming soon

* Ecobee4 + sensors for upstairs
* Z Wave dimmer for back porch lights plus motion sensor for security
* Z Wave switch for fireplace
* Randomize Hue Bloom colors each time a scene triggers them from off to on
* More accurate and frequent presence detection
