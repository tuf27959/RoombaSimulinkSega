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

**Bump Sensor Library**
![Bump Sensor Library](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Project2/Figures/Bump_Sensor_Library.png)
- The Bump has five local sensors Front Bump, Left bump, Right Bump, Left wheel drop, and Right wheel drop.
- The block has one input which the controller and one output Bump size 5 double.
- Bump send a 1 for each sensor activated.

**Alarm Library**

![Alarm Library](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Project2/Figures/Alarm%20Library.png)
- The Alarm Library Plays a short beep tone.

**Example File**

![Example File](https://github.com/tuf27959/RoombaSimulinkSega/blob/master/Project2/Figures/Project2.png) 
- The Example file show the sensor libraries conections and how the all those output control the roomba.
