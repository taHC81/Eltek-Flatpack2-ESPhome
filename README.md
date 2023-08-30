# Eltek-Flaptak2-ESPhome
Configure and monitor Eltek Flaptak2 PSU using ESPhome, here used to charge Li-ion battery pack, controlled from Home assistant.

## HW prototype
- WEMOS D1 MINI ESP32
- SN65HVD230 CAN transciver

## Notes
- note that PSU is reverting to the default voltage with no current limit while the communication is lost
- CAN bus is wired directly from the PSU, you shall use "professional" board to connect the backplane

![HW](https://github.com/taHC81/Eltek-Flaptak2-ESPhome/blob/main/FP2-ESPhome2.jpg?raw=true)
![HW](https://github.com/taHC81/Eltek-Flaptak2-ESPhome/blob/main/FP2-ESPhome1.jpg?raw=true)

## How it should looks like within the Home assistant lovelace
![HA lovelace](https://github.com/taHC81/Eltek-Flaptack2-ESPhome/blob/main/Eltek-Flatpack2-HA2.png?raw=true)
