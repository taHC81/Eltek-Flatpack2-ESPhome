# Eltek-Flatpack2-ESPhome
Configure and monitor Eltek Flatpack2 PSU using ESPhome, here used to charge Li-ion battery pack, controlled from Home assistant.

## HW prototype
- WEMOS D1 MINI ESP32
- SN65HVD230 CAN transceiver

## Sources
https://openinverter.org/forum/viewtopic.php?t=1351

## Notes
- note that PSU is reverting to the default voltage with no current limit while the communication is lost
- CAN bus is wired directly from the PSU, you shall use "professional" board to connect the backplane
- there's a layer of insluating tape (polyimide, kapton) below the CAN transceiver
- update serial number with your own (see the CAN message 0x05004804)
- current limiting is working only above 48V on an output terminals (not just configured voltage)

![HW](https://github.com/taHC81/Eltek-Flaptak2-ESPhome/blob/main/FP2-ESPhome2.jpg?raw=true)
![HW](https://github.com/taHC81/Eltek-Flaptak2-ESPhome/blob/main/FP2-ESPhome1.jpg?raw=true)
![Serial number](https://github.com/taHC81/Eltek-Flaptak2-ESPhome/blob/main/ELTEK-FP2-serial.jpg?raw=true)
## How it should looks like within the Home assistant lovelace
![HA lovelace](https://github.com/taHC81/Eltek-Flaptack2-ESPhome/blob/main/Eltek-Flatpack2-HA2.png?raw=true)
