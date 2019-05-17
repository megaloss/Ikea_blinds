This is the source code for Ikea rollerblind with my commits.
Thanks to https://github.com/danjperron/ESP12EMotorShieldRollerBlind for stepper.lua code.
Building hardware is described here: https://www.instructables.com/id/Motorized-WiFi-IKEA-Roller-Blind

To connect step motor read comments in stepper.lua !!!

Motor is to be placed on the right side of a blind, remove the nut from a spring stopper inside a blind tube.
To upload code to ESP8266 uncheck "Autodetect firmware", select speed 115200.
File cfg_tot_steps.lua contains total number of steps, in my case 27000 steps for 120cm blind.

I use Home Assistant to control blinds through MQTT protocol
Here is a link to setting guide: 
https://www.home-assistant.io/components/cover.mqtt/

To establish a link with Google Assistant read here: 
https://www.home-assistant.io/components/google_assistant/
you will need to expose your port (8123) to internet.
read here:
https://www.home-assistant.io/components/duckdns/

For voice control say "open/close curtains", "open curtains to 50%".
