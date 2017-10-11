# RoombaSimulinkSega
**Sega Diallo**
```
These libraries are for controlling iRoomba wheels and IR sensor using Wifi module 10.0.0.1
I incorporate a real-time pacer to be able to see the changes.
```
**Main Switch Library**
![Main Switch Block](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Main%20Switch%20Library.png)
- This block establish the connection between Simulink and the Roomba.
- It communicate by using the with the Wifi module using the tcpip function 
- Input 1 turn ON and input 0 turn OFF
- The output toggle between the two secondary blocks
**Wheel Control Library**
![Main Switch Block](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Wheel%20Control%20Library.png)
- The Wheel Control library has three inputs and one output
- Left Wheel and Right Wheel inputs control the linear speed of the wheel
- inputv is the output from the Main Switch Library
- The Status output show the Status of the library Block
