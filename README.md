# Home Assistant Config

![Home Assistant front-end](http://i.imgur.com/buFzIfi.png)

Hey! This is my Home Assistant configuration. Here's what my setup entails so far:

# Devices

Here's the stuff I use.

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

## Misc
* Ecobee3 smart thermostat + sensors
* Simplisafe wireless home security system
* LiftMaster CIGBU Internet Gateway for MyQ garage door
* Amazon Echo
* Amazon Echo dot

# Automations

* Turn on outside lights at sunset
  - If cloud cover is over 75%, turn them on 2.5 hours before sunset (because it's darker)
  - If cloud cover is under 75%, turn them on only 30 minutes before sunset (because it's brighter)
* Simplisafe alarm-controlled automations
  - Disarm the alarm every morning at 6:45 AM, turn on morning light scene
  - When alarm is manually armed at night, turn on nighttime light scene
  - If alarm siren is activated, flash all controlled lights in house once per second until disarmed
* When Apple TV is playing, trigger media light scene
* When Apple TV is paused, trigger media-paused light scene
