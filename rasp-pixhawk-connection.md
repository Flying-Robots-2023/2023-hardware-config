# Solving Connection Problems

## Configuring permission of ports

We used the following links as reference:

https://medium.com/@andy.hwang/ttys0-permission-denied-on-ubuntu-mate-18-04-on-raspberry-pi-3b-3230ad303e96

https://answers.ros.org/question/220319/ros-run-mavros-with-permission-denied/

## Connection between RaspberryPi4 and Pixhawk

We did the connections using jumpers as shown in [px4-guide](https://docs.px4.io/main/en/companion_computer/pixhawk_rpi.html)

We had a problem with the fcu_url connection between the RaspberryPi 4b and The Pixhawk using mavros. To solve this, we follow the tutorial of this [link](https://devicetests.com/enabling-uart-communication-raspberry-pi-4-ubuntu-20-04).
```
sudo nano /boot/firmware/config.txt
```
Then editing it, so we would have ```enable_uart=1``` on the script.

```
sudo nano /boot/firmware/cmdline.txt
```
We removed ```console=serial0,115200``` from the  line.
