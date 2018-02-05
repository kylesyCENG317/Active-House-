---
tagline: Website with GitHub Pages
description: Simple website with GitHub Pages
layout: page
title: simple site
---
Robotic Vaccuum
KYLE SY BLOG.
-------------

### Week 12
![Image of System Diagram/Introduction](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/system%20diagram.png)


![Image of Budget](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/budget.png)


![Image of Time](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/time%20commitment.png)

Mechanical Assembly

1. Connect the battery pack to the  GND and VCC ports of the motor driver (refer to the system diagram)
2. Connect the motor driver pins to the designated GPIO pins of Raspberry Pi, also make a connection between the motor driver's 5V and GND to the designated GPIO pins of Raspberry Pi
3. Prepare the chassis of our robot.  The problem is with the availability of tools and material. The most ideal material for this project will be Acrylic. The dimensions of the chasis should comply with how the vacuum is going to be integrated. 
4. Mount the Raspberry Pi and the motor driver.
5. Connect the 4 motors to the motor driver. (Refer to the system diagram). After this, the wheels are to be attached to the motor shafts.
6. Make a voltage divider circuit for the Ultrasonic Sensor for it to be compatible to the Raspberry Pi.
7. Connect the Ultrasonic Sensor to the Raspberry Pi's GPIO pins. 
8. The Vacuum Cleaner is the most crucial part in placement of Robot. It has to be placed at tilted angle on the chasis, so that it can provide proper vacuum action
9. Mount the sensors on front of the vacuum cleaner and the sides of the chasis.

![Image of Mech Assmbly](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/mechanical%20Assem.png)

PCB/Soldering

![Image of PCB](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/PCB.png)

Refer to this

Power Up

1. Put the batteries into the battery holder

2. If the H Drive is receiving power from the batteries the LED should illuminate

3. Remove one of the batteries from the battery holder to turn of the motors as you will need to test if the raspberry pi is powering the motor driver

4. Plug in the raspberry pi and the LED on the motor driver should illuminate once again

5. Now put the batteries back into the battery holder and all components should be powered up

Unit Testing

For the motors

1. Power up the raspberry pi and login

2. Use sudo nano fwdback.py on a terminal and write these codes [fwdback.py](https://github.com/Khemar1/khemar1.github.io/blob/master/documentation/fwdback.py):

3. Go to your terminal and go to the directory where you downloaded fwback.py
	
4. Run the program using sudo python fwdback.py

5. If all connections were made correctly then the wheels should move forward and backward

For the sensors

1. Power up the raspberry pi and login

2. Use sudo nano sensor.py on a terminal and write these codes [sensor.py](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/blob/master/sensor.py):
    
3. Open your terminal and go into the directory where you downloaded the program

4. Run the program using the command sudo python sensor.py  
5. Place an object in front of the sensor and it should return the distance of the object to the screen.

Production Testing

The car and the vacuum runs independently of each other. Power up the vacuum first

1. Power up the raspberry pi

2. Put in the batteries

3. Connect the raspberry pi to a remote pc to view the desktop

4. Login to the raspberry pi

5. Open up a terminal and download [auto1.py](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/blob/master/auto1.py):

6. Go to your terminal and navigate to where you downloaded auto1.py. Run the program using sudo python auto1.py

7. Place the car in the open area

8. The car should move forward continuously

9. When the car senses an obstacle it should reverse and change direction(whether it be left or right. This is choses randomly by the program)

10. If it senses an obstacle in the direction it turned to then it will turn once again.

11. The car will continuously do this until it cannot find a path to continue


### Week 11
Created [PowerPoint Presentation](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/blob/master/Robotic%20Vacuum%20PowerPoint%20A.pdf)
### Week 10



Latest Update
 The latest thing I've done is to get my sensor working.At first I had an issue with my sensor because it is giving faulty data. I took care of this issue by following a different model in the internet that shows how to utlize an ultrasonic sensor. This was done by building a circuit the lowers the output voltage of the sensor to something the raspberry pi can handle. Also, I have most of my assembly done; I mounted the motor driver, the motors and the wheels to the chasis already. 
Schedule
 So far, I'm still on track as of the original schedule that has been made. I missed one class where I was supposed to set up my raspberry pi and test the pcb with it. But because of the fact that there is so much time in between of the milestones, I was also able to do this. There were times where I couldn't progress schedule wise because some parts are missing, or some people who I collaborated with aren't on the same page as me, but it's not really that big of a deal. The schedule is pretty much this: project proposal, schedule proposal, budget proposal, acquisition of parts, setting up the raspberry and setting up the sensors and I'm still on top of my game. I'm expecting to finish the prototype on time. 

Problems encountered
 One of the major problems that came for me is the acquisition of materials. Unfortunately I wasn't able to get my hands on them in just one shot. This is because I 'm constantly making modifications on my projects weekly. At this point though, everything is finalized so that shouldn't be a big problem anymore. Another issue would be the fact that there are three people collaborating on this project. We normally work individually and separately and we have yet to integrate everything together and I'm afraid this might be a make or break in terms of finishing the project. We have got all our sensors to work by this point and we have all the parts we need so we just have to commit to communicating eagerly to build the project already.

Budget Updates
 When it comes to the financial department, I have no issues. This is not because I was able to purchase everything that I need but because I was able to cut my budget but also because I had to acquire more parts. Overall, the summation is still to what is expected. Some examples are: being able to make an improvised chasis(a plus), buying a motor driver(a minus since it wasnt included in the original budget plan).



### Week 9 
Made a 30 second video
![video](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/blob/master/first%20part.mp4)
![first part](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/blob/master/video-1513357683%20(1).mp4)
### Week 8
Made a placard


![Image of placard](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/placardvacuum.png)


30 Second Video Script

My name is Kyle and I undertook a robotic vacuum project.This robot is a simple four wheeled vacuum that could smartly avoid obstacles.(2 seconds)

In order to build the robot we would need the following parts:
	wooden sheets for chasis
	IR sensor
	Vacuum cleaner which runs on dc current
	raspberry pi	 
	12v20ah battery
	connecting wires	
	and enthusiastic energy to learn and work 

(7 seconds)
The Vacuum clearner is the most crucial part in placement in the robot. it has to be placed at a tilted angle so that it can provide proper vacuum action.
If everything works fine, we can connect the sensors with the raspberry pi as shown in the diagram. As you can see, the ultrasonic sensor is mounted to the front.
(7 seconds)

The vacuum cleaner is not controlled by the Raspberry pi. Once you power the on the robot, the vacuum is also turned on as seen in the video.
(7 seconds)


The functionality that I plan to demonstrate here is the speed of my car. This is done so that the vacuum action takes place.(7 seconds)




### Week 7
PCB Test Due
testing of the PCB failed. 
Ran a series of test with Kelly but could't figure out the problem.
Raspberry Pi set up successful 
![Image of pi with the pcd embedded on it](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-03-16-57%5B1%5D.png)

### Week 6
Picked up RTC module from the prototype lab



![Image of acquired modules](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-48-16.png) 

soldered the pcb 
![Image of pcb](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-48-30.png) 
![Image of pcb2](![Image of pcb](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-48-24.png) ) 

## Week 5
READING WEEK
Acquired parts for the project 




4 pmdc Motors 
![Image of pmdc motors](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-45-47.png)


battery 12v7ah 
![Image of battery](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-46-04.png)


Raspberry pi
![Image of raspberry pi](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-48-09.png)


Ultrasonic Sensor
![Image of ultrasonic sensor](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Screenshot_2017-12-08-02-45-56.png)


### Week 4
Created a budget proposal
![Image of Proposal](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/Untitled.png)

Reviewed project listing

### Week 3

Created PROJECT SCHEDULE.  
![Image of Schedule](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/sched1.png)

![Image of Schedule](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/sched2.png)

![Image of Schedule](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/sched3.png)

![Image of Schedule](https://raw.githubusercontent.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/master/sched4.png)

### Week 2

Created a [floor scrubber project proposal](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber/blob/master/Proposal%20(1).pdf). 
Parts kit and safety glasses were implemented as a rule; will be checked regulary.

### Week 1

Created [repository](https://github.com/kylesyCENG317/Robotic-Vacuum-and-Floor-Scrubber). Wrote a quiz out of 10 about items that can be embedded with microprocessors.Started brainstroming about Project Proposal which is to be handed in next week. 

### August 30, 2017

Welcome!
