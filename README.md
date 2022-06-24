Lightwaverf intergration for Home Assistant on raspberry pi 4 32 bit

Lightwaverf hub 1st gen

I made a seprate lightwave.yaml file to keep the config one cleen but it can all go into the main one if you wish.

I have now got the Electric Switch LW934 working to contral our emersion heater!

For the Electric Switch LW934      
At the moment the On and Off switches are independant so you have to switch it On using the On switch.
Switch it off by switching the On switch to Off and the Off switch to On.
When switching back On switch the Off switch to Off and the on switch to On.
I will work on an auto script for this in the future.

host: 192.168.x.xxx Enter you lightwaverf hub IP address

lights:
R1D1: R=room number D=device number
name: Master Bedroom Ceiling Light

switches:
R 1F*tP50:
name: Immersion heater Off R 1F*tP50
R 1F*tP60:
name: Immersion heater On R 1F*tP60

References:
https://www.home-assistant.io/integrations/lightwave/
