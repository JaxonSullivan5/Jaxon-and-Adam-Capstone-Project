# Capstone_Project
(Written By: Adam Kirkpatrick and Jaxon Sullivan)

5/10/23

**Design Summary:**

Our arm design is based of the EEZYbotARM by Carlo Franciscone. We liked this design other than the fact that it only incorperated micro servos. So we decided to make the design work for full sized servos that were to be used in the base and we figured we'd make the arm longer to maximize the filament limit. In the end the arm bassically functions by having a servo rotate the whole arm, a sero elevate the arm, and a seperate servo extend the arm. In terms of controlls we simply used the two thumb sticks and their stand that were from the original kit with the orginal model arm. In addition, for our autonomous mode we used the previously mentioned color sensor and a rgb LED to display the color of the object detected. Finally, we used a switch to change betweeen the two different modes.

**System Details:**

This system uses three servos, one for rotation, one for elevation, and one for exntention of the arm. The servo used for rotation is held within the lower base componet while the servos used for elevation and extention are housed in the upper base where one is directly connected to the main arm piece while the other one is connected to an extended servo horn of sorts that in and of itself is connected to the main upper arm section. On the tip of the arm connecting the main and secondary upper sections is the claw section. In this section there is a micro servo that is placed upside down and it is connected to a set of gears that have extensions on them to make the actual pincer of the claw. It is important to note that the color sensor is taped on the front of the micro servo so it can get the most acurate color reading from the object that is being picked up. The rgb LED and the switch that is used for switching between the autonomous and manual modes are both situated on a bread board that is the hub for almost all of our wiring.

**Design Evaluation:**

* This project meets the Output Display requirement via using an rgb LED that returns readings from the color sensor.
* The Manual User input requirement is met by having a manual control mode with two thumb sticks where the used has full controll over the system. User Input is also seen with the switch that allows for the user to switch to the autonomous mode if they so please.
* This project meets the Automatic Sensor requirement because of the aforementioned color sensor that directs the arm to sort objects in predestined locations based on their color.
* The Actuators, Mechanisms, and Hardware requirement is fufilled thanks to the numerous servos, the gears in the claw, and the system of linkages that connects the whole system.
* Our project also meets the Logic, Processing, and Control via having programmed logic with the color sensor based autonomous mode and the calculations achieved to use the sticks in the manual mode.

**Parts List:**

* Three Deegoo-FPV Servos costing $15 dollars in total
 (Model Number MG995)
* One HiTec mircro servo costing $2.50
 (Model Number SG90)
* One HiLetgo color sensor costing $7
 (Model Number TCS34725)
* One ELEGOO MEGA R3 Board ATmega 2560 costing $21
 (Model Number LYSB01H4ZDYCE-ELECTRNCS)
* One HiLetgo bread board costing $2.50
 (3-01-0192)
* WGCD thumbsticks costing $4.80
 (8542140575)
 
 **Lessons Learned**
 
 During this project we learned mostly about how to code the color sensor and the thumb sticks. This process involved (JAXON PUT YOUR LEARNING EXPERIENCE HERE) Secondly, we learned how to use many different tools in onShape to design our parts to be as structurally strong and clean in appearance. Specifically, we heavily used drafts, fillets, and extrudes to make our model have a smooth appearance. We learned how to use the draft for the triangle like piece on the top of the main arm and the extrusion off the upper base. These parts also required partial fillets until we combined their seperate sections by using the boolean function. We used fillets everywhere except for the bottom of the base pieces because we wanted those pieces to sit flat against whatever surface we mounted them on. We extruded all of our parts from the bottom up and removed sections by using horizontal removal extrudes.
