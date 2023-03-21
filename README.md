# CTC-EcoHeat400---Homeassistant
This is a fork of @Kasper-73's repository, all credit to him for doing the hard work. (Ogiginal: https://github.com/kasper-73/CTC-GSi-8---Homeassistant) 

I updated his script with a couple of small fixes, and adapted it to run on an ESP-12F_Relay_X2 board. This adds the option to utilize the EcoHeat Smart A and Smart B inputs, that enable a lot of power saving featurs. I only wonder why CTC hides these features so well.....


For connection between CTC EcoHeat and Homeassistant (testet with CTC EcoHeat 412).
I haven't found all the modbus registers yet from the lists in the pdf files

I added a Dallas temperature sensor as well, connected to GPIO2

![Skærmbillede 2022-11-07 151830](https://user-images.githubusercontent.com/71944008/200332690-383c7424-a406-4df4-b542-bcc13bf7fdfd.png)


RJ12 cable cut in half an connected to ESP-12F

Pinout for the RJ12 cable connected to the display of the CTC heat pump

![image-png-Jun-29-2022-09-29-07-52-AM](https://user-images.githubusercontent.com/71944008/200346393-598ecfbc-5bc0-45ca-adbf-1e089296bc18.png)

1: GND

2: 5V

3: Not used

4: RX GPIO 13

5: Flow control pin GPIO 12 

6: TX GPIO 14

![IMG_7518](https://user-images.githubusercontent.com/58219639/226720655-22fad034-ee9d-42ee-974b-83147a12c1c2.jpg)


Using Esphome it is possible to read and write modbus.
