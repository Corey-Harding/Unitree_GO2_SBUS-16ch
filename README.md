<pre>
 SPY ON SBUS in SSH Session

/unitree/sbin/mscli stop sbus_handle
/unitree/module/sbus_handle/sbus_handle

Be sure to restart the sbus_handle before you exit ssh session or you will lose sbus until you restart the service

16 Channel Notes

userCmd: 1
Crouch

userCmd: 2
Stand

userCmd: 3
Damping Mode

userCmd: 3
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
CH11 712 -> 272 -> 1712

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
</pre>

A basic Arduino Sketch to control a Unitree GO2 using the SBUS port.
This uses the follwing libraries:

Bluepad32 - Bluetooth controllers
 - https://github.com/ricardoquesada/bluepad32

Bolder Flight SBUS - Read and write SBUS commands
 - https://github.com/bolderflight/sbus

Requirements:
- XBox Controller with BLE
- ESP32 - Tested With ESP32S3
- Buck Converter - LM2596 Used
- XT30 Male Power Connector
- 3P 1.25mm Picoblade

[![Video](https://img.youtube.com/vi/AR2y-QA6O1I/0.jpg)](https://www.youtube.com/watch?v=AR2y-QA6O1I)
