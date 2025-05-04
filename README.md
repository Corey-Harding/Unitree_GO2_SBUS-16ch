```
For a working 8ch implementation use the original creators fork here: https://github.com/mechzrobotics/Unitree_GO2_SBUS

This fork is for research and development towards getting the 16ch implementation working.
Hopefully bringing with it additional commands that are not available on the 8ch implementation.
 
 SPY ON SBUS in SSH Session

/unitree/sbin/mscli stop sbus_handle
/unitree/module/sbus_handle/sbus_handle

Be sure to restart the sbus_handle before you exit ssh session or you will lose sbus until you start the service

/unitree/sbin/mscli start sbus_handle


16 Channel Notes

userCmd: 1
Crouch

userCmd: 2
Stand

userCmd: 3
Damping Mode

userCmd: 4
Fall Recover

userCmd: 5
Unlock/Change Walking State
CH13 1712 -> 992 -> 1712

userCmd: 7
Continuous Motion
CH13 1712 -> 1500 -> 1712

userCmd: 8
Obstacle Avoidance On
CH10 1712 -> 272 -> 1712

userCmd: 9
Obstacle Avoidance Off
CH11 1712 -> 272 -> 1712

userCmd: 14
Dance

userCmd: 19
Normal Gait(Walk)

userCmd: 20
Run

userCmd: 21
Climb

userCmd: 22
Spotlight On
CH5 992 -> 272 -> 992
CH12 992 -> 1500 -> 992

userCmd: 23
Spotlight Off
CH5 992 -> 272 -> 992
CH12 992 -> 1500 -> 992

userCmd: 24
Jump

A basic Arduino Sketch to control a Unitree GO2 using the SBUS port.
This uses the follwing libraries:

Bluepad32 - Bluetooth controllers
 - https://github.com/ricardoquesada/bluepad32

Bolder Flight SBUS - Read and write SBUS commands
 - https://github.com/bolderflight/sbus

AsyncTCP
 - https://github.com/ESP32Async/AsyncTCP

ESPAsyncWebServer
 - https://github.com/ESP32Async/ESPAsyncWebServer

 ElegantOTA
  - https://github.com/ayushsharma82/ElegantOTA

Requirements:
- XBox Controller with BLE
- ESP32 - Waveshare ESP32-S3-Zero
- Buck Converter - LM2596 Used
- XT30 Male Power Connector
- 3P 1.25mm GH Connector
```
