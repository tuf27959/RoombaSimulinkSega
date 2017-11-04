# RoombaSimulinkSega
**Sega Diallo Temple University School of Engineering**
```
These libraries are for controlling iRoomba wheels and IR sensor using Wifi module 10.0.0.1
here is the link to purchase the wifi module: http://www.roowifi.com/products-page/
I incorporate a real-time pacer to be able to see the changes.
```
**Main Switch Library**
![Main Switch Block](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Main%20Switch%20Library.png)
- This block establish the connection between Simulink and the Roomba.
- It communicate by using the with the Wifi module using the tcpip function 
- Input 1 turn ON and input 0 turn OFF
- The output toggle between the two secondary blocks

**Wheel Control Library**
![Wheel Control library](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Wheel%20Control%20Library.png)
- The Wheel Control library has three inputs and one output
- Left Wheel and Right Wheel inputs control the linear speed of the wheel
- inputv is the output from the Main Switch Library
- The Status output show the Status of the library Block

**Sensor Test Library**

![Sensor Test Library](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Sensor%20Test%20Library.png)
- The inputv is received from the main switch block
- The display will display a 1 if there is an obstacle blocking the sensor

**Alarm Library**

- The Alarm Library Plays a short beep tone.

**Example File**

![Example File](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Example%20File.png)
- The example file show the running simulink blocks when the switch is ON 
- The display for the Sensor block sensor 5 with an obstacle and state 1
- The display for wheel block have the right wheel rotating ccw -0.1 and the left wheel rotating cw 0.1
