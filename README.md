[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/kzkUPShx)
# a14g-final-submission

    * Team Number: 12
    * Team Name: Gamers
    * Team Members: Runjun Zhang && Xiwen Lai
    * Github Repository URL: https://github.com/ese5160/a14g-final-submission-t12-gamers.git
    * Description of test hardware: (development boards, sensors, actuators, laptop + OS, etc) 

## 1. Video Presentation
Google drive Link:
https://drive.google.com/file/d/1bUj7KIa1Va4nG0Es5bZDXANIMS4BUluH/view?usp=sharing

## 2. Project Summary
* Device Description:

In the beginning, we had an anomaly in the data from our sensor heartbeat sensor, although the sensor was configured correctly, his data was strange. Later we realized it was due to the lack of filtering part in our code, we found a similar project by searching, our filtering part referred to the design method of their open source project, finally we got the filter we wanted and got the data we wanted.

* Inspiration:

We firmly believe that developing this project is an enriching and engaging endeavor. Throughout this process, we have acquired a substantial amount of new knowledge, which has further inspired and motivated us to bring this project to completion.

* Device Functionality:

1. Explain how your Internet-connected device is designed
The hardware project involves creating smart IoT grips designed for interaction and communication with a computer/phone via Wi-Fi. The grips incorporate a 3-axis accelerometer(LIS2DH12) as the primary sensor, capable of recognizing displacement and attitude changes. This sensor feeds data to the MCU (SAMW25) for processing.

We design a software system consisting of 3 parts: 
* A driver on Windows platform that could receive the data from the game controller we designed and convert the data to basic commands(pitch and roll information) that can be utilized by games or other softwares and send feedbacks back to the controller.
* A Heat rate sensor is used to detect the user information when the put their fingers on it, it could make the grid have a wider range of using, for example, we could use heart rate to detect if the person is sleepy or tired.
* A push button is design to interacte with the remote control, and the remote website could give a feedback by trigering the virbration motor. 

![image](https://github.com/ese5160/a14g-final-submission-t12-gamers/blob/main/img/detail.png)

2. Include sensors, actuators, and other critical components.
* IMU:3-axis accelerometer(LIS2DH12);
* Hearrate sensors: LIS2DH12;
* Vb motor: Vibrating Mini Motor Disc(ADA1201);
* Push button;
* MCU: SAMW25 microcontroller;

3. Challenges
Where did you face difficulties? This could be in firmware, hardware, software, integration, etc.
When we try our buck convert, we find that one of the wire connect to the wrong pin which make the whole converter not working at all.

How did you overcome these challenges?:

To address this, we detached the original pins and reattached them correctly using a new wire. During this process, we accidentally broke one of the pins. Lacking sufficient spare components and faced with this setback, we decided to purchase the necessary equipment ourselves from DigiKey's website. We expedited the shipment to our school, which enabled us to successfully resolve the issue and get this part of the circuit working.

* Prototype Learnings
What lessons did you learn by building and testing this prototype?

Ans: Be sure to double-check that the schematic is correct or it can cause a lot of problems.

If you had to build this device again, what would you do differently?

Ans: We would modify our buck boost circuit to make it more powerful, so that we can add more sensors and we do not need to use the additional wires on the PCB.

* Next Steps
What steps are needed to finish or improve this project?
We would try to do FFT on the heart rate sensors, and it could make the data more obvious.

* Takeaways from ESE5160
What did you learn in ESE5160 through the lectures, assignments, and this course-long prototyping project?
Firstly, we learn the process of designing a PCB board, and also what do we need to consider while doing our design.
Secondly, we learn how to write drives to a sensors we want. Also, we learn how to build a bootloader and use it to upload our firmwares.
Finally, we received a lots of debuging experiences in this whole process. 

* Project Links
Node-red JASON file is in the folder "node-red" 
Red node ui : http://172.178.40.45:1880/ui/

Include a link to your A12G code repository:
https://github.com/ese5160/a12g-firmware-drivers-t12-gamers.git

* Provide the share link to your final PCBA on Altium 365.
Link: https://upenn-eselabs.365.altium.com/designs/6F144891-7E70-4AA1-A882-C6F19E6495C9


## 3. Hardware & Software Requirements
Our goal is to make smart Iot grips for gaming, the main function of the grips is to interact by recognizing its own state and feeding back to the computer via Wi-Fi.

In our initial design, it includes an IMU,a heartrate sensor, a motor, a user push button and an OLED. We finished most of the hardware design implementation except the OLED. 

The reason that we do not finish all our hardware design is that our OLED screen is not arrived with other devices. It may lost on the way, and it is a pity that we didn't have enough time to reorder one.

We successfully drive all the sensors, and also finished the data analysis part. We successfully use the IMU data to calculate the pitch roll information of the grid. We also successfully to design a low pass filter to get the correct heartrate data that we want. What's more, we also create a good user interface to demo our design. The user button could interact with the remote website and the website would drive the button when some unexpected state happens, such as if we roll the grid too much.



## 4. Project Photos & Screenshots
<img src="https://github.com/ese5160/a14g-final-submission-t12-gamers/blob/main/img/Weixin%20Image_20240506163001.jpg" width="15%"></img> <img src="https://github.com/ese5160/a14g-final-submission-t12-gamers/blob/main/img/Weixin%20Image_20240506163019.jpg" width="15%"></img> <img src="https://github.com/ese5160/a14g-final-submission-t12-gamers/blob/main/img/Weixin%20Image_20240506163028.jpg" width="15%"></img> <img src="https://github.com/ese5160/a14g-final-submission-t12-gamers/blob/main/img/Weixin%20Image_20240506163035.jpg" width="15%"></img> <img src="https://github.com/ese5160/a14g-final-submission-t12-gamers/blob/main/img/Weixin%20Image_20240506163042.jpg" width="15%"></img>