# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1:
Initiate the MobileRobot
<br/>

Step2:
Connect your PC with the MobileRobot.
<br/>

Step3:
Open Python program.
<br/>

Step4:
Program the movements of the robot using python code.
<br/>

Step5:
Execute the python program.
<br/>

## Program
```
Python control code to move the mobilerobot along the predefined path.

Developed by: ROSHINI RK

Register No.: 212222230123

```
```
from robomaster import robot
import time
from robomaster import camera


if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

   
    
    ep_chassis.move(x=2.8, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=100,b=0,effect="on")


    ep_chassis.move(x=0 , y=0, z=50, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=255,b=204,effect="on")


    ep_chassis.move(x=0.4, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")


    ep_chassis.move(x=0, y=0, z=45, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=204,b=0,effect="on")


    ep_chassis.move(x=0.8, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=255,effect="on")


    ep_chassis.move(x=0, y=0, z=85, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=128,g=0,b=0,effect="on")



    ep_chassis.move(x=1.2, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

   
    ep_chassis.move(x=0, y=0, z=-45, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=1.7, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=102,g=0,b=202,effect="on")


    ep_chassis.move(x=0, y=0, z=43, xy_speed=1).wait_for_completed()


    ep_chassis.move(x=1.4, y=0, z=0, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=95, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")


    ep_chassis.move(x=2.2, y=0, z=0, xy_speed=1).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=80, xy_speed=1).wait_for_completed()

    ep_led.set_led(comp = "all",r=255,g=102,b=0,effect="on")

    ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1).wait_for_completed()

    time.sleep(4)
    
    
    p_camera.stop_video_stream()
    print("Stopped video streaming.....")
    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)
## Starting point:
![244121923-12b53294-6293-42a6-9544-5c4e7d7c4cc2](https://github.com/roshiniRK/mobilerobot-openloopcontrol/assets/118956165/7c3964ce-b162-46ba-a043-d4fdb930ca5f)
<br/>
## Turning point:
![244122073-97b29097-c9fd-44c4-a1eb-afc0dc392347](https://github.com/roshiniRK/mobilerobot-openloopcontrol/assets/118956165/788cc4f3-b471-4671-becc-01fa75da365b)
<br/>
## End point:
![244122221-05213b9c-0e4b-475d-a6b0-6c93d592c600](https://github.com/roshiniRK/mobilerobot-openloopcontrol/assets/118956165/c7a391f3-6de8-48cb-8bd4-d5ae63dc2de4)
<br/>

## MobileRobot Movement Video:

https://youtu.be/xG8uLQ4aqBk
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
