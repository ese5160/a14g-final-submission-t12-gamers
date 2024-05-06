[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/kzkUPShx)
# a14g-final-submission

    * Team Number: 12
    * Team Name: Gamers
    * Team Members: Runjun Zhang && Xiwen Lai
    * Github Repository URL: https://github.com/ese5160/a14g-final-submission-t12-gamers.git
    * Description of test hardware: (development boards, sensors, actuators, laptop + OS, etc) 

## 1. Video Presentation

## 2. Project Summary
* Device Description
    What problem is your device solving? How do you use the Internet so augment your device functionality?
* Inspiration
○	What inspired you to do the project?
* Device Functionality
○	Explain how your Internet-connected device is designed
○	Include sensors, actuators, and other critical components.
○	Your block diagram from earlier in this semester will be quite helpful here!
* Challenges
○	Where did you face difficulties? This could be in firmware, hardware, software, integration, etc.
○	How did you overcome these challenges?
* Prototype Learnings
○	What lessons did you learn by building and testing this prototype?
○	If you had to build this device again, what would you do differently?

* Next Steps
○	What steps are needed to finish or improve this project?
* Takeaways from ESE5160
○	What did you learn in ESE5160 through the lectures, assignments, and this course-long prototyping project?
* Project Links
○	Provide a URL to your Node-RED instance for our review (make sure it’s running on your Azure instance!)
○	Include a link to your A12G code repository
Do NOT put your code in the A14G assignment’s repository. 
The A12G repository must include your final embedded C firmware codebases and Node-RED dashboard code.
Your code will be evaluated for its driver implementations, application code, OTAU approach, comments, and cleanliness.
If any open source code was used in your project, it must be referenced and used according to its licensing information. If you heavily leveraged tools, websites, or the expertise of others, this must be noted in the Github Readme.
○	Provide the share link to your final PCBA on Altium 365.
■	Consider downloading your PCBA source and manufacturing files to keep after you leave UPenn. Your Altium access will expire after this semester.

## 3. Hardware & Software Requirements
Our goal is to make smart Iot grips for gaming, the main function of the grips is to interact by recognizing its own state and feeding back to the computer via Wi-Fi.

In our initial design, it includes an IMU,a heartrate sensor, a motor, a user push button and an OLED. We finished most of the hardware design implementation except the OLED. 

The reason that we do not finish all our hardware design is that our OLED screen is not arrived with other devices. It may lost on the way, and it is a pity that we didn't have enough time to reorder one.

We successfully drive all the sensors, and also finished the data analysis part. We successfully use the IMU data to calculate the pitch roll information of the grid. We also successfully to design a low pass filter to get the correct heartrate data that we want. What's more, we also create a good user interface to demo our design. The user button could interact with the remote website and the website would drive the button when some unexpected state happens, such as if we roll the grid too much.



## 4. Project Photos & Screenshots
