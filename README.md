# Home Assistant Config

Hey! This is my Home Assistant configuration. Under the screenshot of my Home Assistant front-end, you'll find the devices I'm using, the automations I have running, as well as some video examples.

![Home Assistant front-end](http://i.imgur.com/buFzIfi.png)

# Devices

Here's the stuff I use to control my home. It's a mixture of Z Wave and Wifi devices, all controlled by Home Assistant and the Amazon Echo for voice.

## Controller
* Raspberry Pi 3 running Home Assistant
* Aeotec ZW090 Z Stick

## Switches and lights
* GE Z-Wave Smart Dimmer Toggle Switch 12729 (x6)
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
* Turn all lights on when wife and kids leave for school
* Turn on evening light scene at 4:30 PM every day
* Turn off all lights at midnight
* Turn on and off lights (independently or as a group) using Alexa [[video example]](https://youtu.be/am7hBSraAyA)

## Security
* Disarm the alarm every morning at 6:45 AM, turn on morning light scene
* When alarm is manually armed at night, turn on nighttime light scene
* If alarm siren is activated, flash all controlled lights in house once per second until disarmed [[video example]](https://youtu.be/K4GNwNoDph4)
* Send mobile alert when garage door opens

## Media

* When Apple TV is playing, trigger media light scene
* When Apple TV is paused, trigger media-paused light scene
