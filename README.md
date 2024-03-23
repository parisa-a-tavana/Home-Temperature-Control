![pi_controller_real](https://github.com/parisa-a-tavana/Home-Temperature-Control/assets/104492285/c981cce7-28c5-4f17-8975-8fb610483db2)# Home-Temperature-Control
<br>
In this project, we want to control the indoor temperature of which is effected by the outdoor temperature and the heater.
<br>
![Image 1](images/open_loop.jpg)
<br>
<br>

__Actuator__:
<br>
![Image 2](images/actuator.jpg)
<br>
Q: output heat
<br>
V: input voltage
<br>
<br>
__Sensor__:
<br>
![Image 3](images/sensor.jpg)
<br>
Ts: the measured temperature
<br>
Vout: output voltage
<br>
<br>
__Heater Driver__:
<br>
![Image 4](images/heater_driver.jpg)
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
![Image 5](images/sensor_optimizer.jpg)
<br>
<br>
__Open Loop Controller__:
<br>
The desired temperature is 26 C and the current temperature of th house is 68.38 C. We use a simple gain as a controller. 
<br>
![Image 6](images/openloop_controller.jpg)
<br>
![Image 7](images/openloop_controller_diagram.jpg)
<br>
<br>
__Closed Loop Controller__:
<br>
We design a PI controller that sets T=26 C in less that 40s without overshoot.
<br>
![Image 8](images/pi_controller.jpg)
<br>
![Image 9](images/pi_controller_real.jpg)
<br>
![Image 10](images/pi_controller_diagram.jpg)
<br>
![Image 11](images/pi_controller_diagram_vout.jpg)
<br>
We also impliment the controller using LM324. 
