# Home-Temperature-Control
<br>
In this project, we want to control the indoor temperature of which is effected by the outdoor temperature and the heater.
<br>

__Actuator__:
<br>
![Image 1](images/system.jpg)
<br>
Q: output heat
<br>
V: input voltage
<br>
<br>
__Sensor__:
<br>
![Image 2](images/system.jpg)
<br>
Ts: the measured temperature
<br>
Vout: output voltage
<br>
<br>
__Sensor Optimizer__:
<br>
we use LM358 IC to map the sensor output amplitude to the input.
<br>
![Image 2](images/system.jpg)
<br>
<br>
__Open Loop Controller__:
<br>
The desired temperature is 26 C and the current temperature of th house is 68.38 C. We use a simple gain as a controller. 
<br>
![Image 2](images/system.jpg)
<br>
![Image 2](images/system.jpg)
<br>
<br>
__Closed Loop Controller__:
<br>
We design a PI controller that sets T=26 C in less that 40s without overshoot.
<br>
![Image 2](images/system.jpg)
<br>
![Image 2](images/system.jpg)
<br>
We also impliment the controller using LM324. 
