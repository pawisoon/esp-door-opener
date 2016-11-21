# esp-door-opener

#Parts:
  - ESP8266 (any version) 
  - Transistor PNP2222/A
  - Resistor 220 Ohm
  - A couple of wires(I recommend 30AWG)
  
#SETUP
- Connect your esp with power supply and make sure everything is connected as on the schema in this repo or as on the picture below. 


<schema to be uploaded>


- Upload the sketch.

- Setup redirection route on your router. If you have static IP you are sorted, in case you dont you probably have raspberry pi / beaglebone connected to your network - setup a ddns service on it. 


- In your router setup: 

  1. Go to Port forwarding 

  2. Depending on your router software this table will look a bit different but it's all the same. 
Set it up in this way: 
https://scr.hu/RLY5J6

  3. Save config and try it in your browser. 
  4. Go to: yourip:4001 or hostname.com:4001 (in case you are using ddns on rpi you will have to edit port forwarding a little bit so it will handle request and pass it to ESP via your LAN)

  5. Your door should open now :) 
