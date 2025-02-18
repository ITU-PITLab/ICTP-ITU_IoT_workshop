## Building a RAK2245 Gateway

Documentation:

https://downloads.rakwireless.com/en/LoRa/RAK2245-Pi-HAT/

The guide is here:

https://downloads.rakwireless.com/en/LoRa/RAK2245-Pi-HAT/Application-Notes/Get_Start_with_RAK2245%26RAK831_RPi_LoRa_Gateway.pdf


**Note: In the AIT Interlab workshop, steps 1 + 2 have already been done for you! You may thank Adisorn!** 


### 1. Physical Assembly

Put the PiHat onto the Raspberry Pi, assemble enclosure.

See here:

https://www.hackster.io/makoooy123/unboxing-rak-wireless-rak2245-lora-starter-kit-c18dbf

### 2. Prepare SD card

Download Operating System Image from here

https://downloads.rakwireless.com/en/LoRa/RAK2245-Pi-HAT/

and burn onto SD card

Help needed fro burning SD card? ==> 
https://www.raspberrypi.org/documentation/installation/installing-images/

----

### 3. Connect to the Raspberry Pi via ssh

See guide for help and IP information.


### 4. Configure the Raspberry Pi

Most important steps:

Run

```
sudo gateway-config
```

and choose which LoRaWAN network server to use -

Either TTN (TheThingsNetwork)

or

any other of your own choice .


Remember to write down your GatewayID.
You can get it at all times by running
```
gateway-version
```

Important: Choose how we connect the Raspberry Pi to the Internet.

Our choice:

* Keep Wi-Fi AP running for now

* Set static IP for ethernet interface:
```
		10.15.222.10.x with x = group number
```



### 5. Add your gateway to TTN

Go to https://TheThingsnetwork.org,

create an account for yourself, log on an follow the guide.
