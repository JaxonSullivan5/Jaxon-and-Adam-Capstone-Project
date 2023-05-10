# Robotic Arm Capstone Project
(Written By: Adam Kirkpatrick and Jaxon Sullivan)

5/10/23


(Figure 1: Picture of Finished Arm)

**Design Summary:**

Our arm design is based off of the EEZYbotARM mk1 made by Carlo Franciscone. We like this design except for the fact that it only incorporates micro servos as opposed to using full sized servos. So we decided to make the design work for full sized servos that were to be used in the base and we figured we'd make the arm longer to maximize the filament limit. In the end, the arm basically functions by having a servo rotate the whole arm, a servo elevate the arm, and a separate servo extend the arm. In terms of controls we simply used the two thumb sticks for moving the arm and using the claw. (One stick controlls rotation/elevation, and the other stick controls extension/grabbing via the button inside the stick. In addition to the manual mode, we have an autonomous mode were we use a color sensor to give information to the servos (so they can sort objects based on thier color) and a rgb LED to display the color of the object detected. Finally, we used a switch to change between the two different modes.

![Screenshot 2023-05-10 7 01 51 AM](https://github.com/JaxonSullivan5/Jaxon-and-Adam-Capstone-Project/assets/99275889/0bbcb154-71bc-4c67-937c-7d67f1c473c3)
(Figure 2: Original EEZYbotARM mk1 made by Carlo Franciscone.)

**System Details:**

This system uses three servos, one for rotation, one for elevation, and one for exntension of the arm. The servo used for rotation is held within the lower base component while the servos used for elevation and extension are housed in the upper base where one is directly connected to the main arm piece while the other one is connected to an extended servo horn piece that in and of itself is connected to the main upper arm section. On the tip of the arm connecting the main and secondary upper sections is the claw section. In this section there is a micro servo that is placed upside down and it is connected to a set of gears that have extensions on them to make the actual pincer of the claw. It is important to note that the color sensor is taped on the front of the micro servo so it can get the most accurate color reading from the object that is being picked up. The rgb LED and the switch that is used for switching between the autonomous and manual modes are both situated on a breadboard that is the hub for almost all of our wiring.

![IMG-9178](https://github.com/JaxonSullivan5/Jaxon-and-Adam-Capstone-Project/assets/99275889/ee6b92a0-0d28-497e-9008-0f556b7afe6d)
(Figure 3: Picture of extended servo horn, main lower beam, main upper beam, and triangular beam in order from farthest to closest.)

**Design Evaluation:**

* This project meets the Output Display requirement via using an rgb LED that returns readings from the color sensor.
* The Manual User input requirement is met by having a manual control mode with two thumb sticks where the used has full controll over the system. User Input is also seen with the switch that allows for the user to switch to the autonomous mode if they so please.
* This project meets the Automatic Sensor requirement because of the aforementioned color sensor that directs the arm to sort objects in predestined locations based on their color.
* The Actuators, Mechanisms, and Hardware requirement is fufilled thanks to the numerous servos, the gears in the claw, and the system of linkages that connects the whole system.
* Our project also meets the Logic, Processing, and Control via having programmed logic with the color sensor based autonomous mode and the calculations achieved to use the sticks in the manual mode.

![s0ic0gcptmxqpj12s85jhcdotcco](https://github.com/JaxonSullivan5/Jaxon-and-Adam-Capstone-Project/assets/99275889/e3746fe6-fec4-45f2-8306-8ce36f90db0a)
(Figure 4: Close-Up picture of a Deego-FPV servo)

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
 (Model Number 3-01-0192)
* WGCD thumbsticks costing $4.80
 (Model Number 8542140575)
* EDGELEC rgb LED costing $0.09
 (Model Number ED_YW05_RGB-4P-C)
 TOTAL COST: $52.89

(Note: You will obviously also need all of the 3d printed parts which you can print via the stl files in this repository.)

 **Lessons Learned**
 
 During this project we learned mostly about how to code the color sensor and the thumb sticks. This process involved copying sample code for these components, modifying said code, and then integrating it into the system. This was difficult when we had to merge our autonomous and manual modes. Secondly, we learned how to use many different tools in onShape to design our parts to be as structurally strong and clean in appearance. Specifically, we heavily used drafts, fillets, and extrudes to make our model have a smooth appearance. We learned how to use the draft for the triangle like piece on the top of the main arm and the extrusion off the upper base. These parts also required partial fillets until we combined their seperate sections by using the boolean function. We used fillets everywhere except for the bottom of the base pieces because we wanted those pieces to sit flat against whatever surface we mounted them on. We extruded all of our parts from the bottom up and removed sections by using horizontal removal extrudes. We were going to make a custom claw piece in addition to the rest of our parts; however, we didn't get the chance to do so because of time constraints. Instead, we just used the orginal claw piece because is suites our purposes well enough. My recomendation to any future robotics student is to not overcomplicate your 3d modeled designs unless you have the time to make them look and function perfectly.
 
![Screenshot 2023-05-10 7 48 10 AM](https://github.com/JaxonSullivan5/Jaxon-and-Adam-Capstone-Project/assets/99275889/bd846c3f-ae16-46bf-96ac-c483dc95b708)
(Figure 5: Screenshot highlighting the use of drafts and fillets on the triangular beam in particular)

 **Instructions for assembly**

1. You will need all of the parts listed above in the parts list along with some wires, 220 resistors, a 0.5 cm brass pipe that will be cut to be 3.5 centimeters long, 0.4 centimeter screws, and 0.4 centimeter nuts. All of your screws thould be roughly 1.5 centimeters long except for one screw which should be about 3.5 centimeters long. (Note that you will need a screw driver and/or a wrench of some sort to secure the parts in addition to some tape or hot glue.) 

2. Make sure you have all the 3d printed parts which include 3 small long beams, the main lower beam, the extended servo horn beam, the main upper beam, the triangular beam, and the claw pieces. 

3. Assemble your arm by following these simple steps:

* First, drop your servo into the bottom base piece and screw it in, make sure you feed the wire out of the holes provided so the the arm sits flat on the table.

* Next, attach whatever t shaped servo horn that came with your servo to the previously mentioned servo and then place the top base piece onto it. (There is a box that the servo horn should fit into.)

* Then secure the servo horn to the top base via tape or hot glue.
* Proceed to fit your other two servos into the sides of your top base and secure them with screws.

* Advance by fitting the servo horns into the servos and then putting them into the main lower beam and extended servo horn pieces respectively. (Note that the side with the extended servo horn should be opposite to the upper base with the frontal extrustion.

* Continue via sliding the brass pipe through the extended servo piece, the central extrusion, and the main beam. Make sure that it's as tightlu fitted as posible from one servo horn to anather.

* Then put the triangular beam in the smaller of the two top notches in the main beam, ensure that the elevated and shortest extrusion is facing away from the top base's extrusion.

* Begin to put the main upper beam into the bigger notch of the main lower beam. Make sure the middle hole of the main upper beam is the on lined up with the holes of the triangular piece and the main lower beam. Then you can fit your long 3.5 centimeter screw through all three of these parts. (Note: The longer side of the main upper beam should face the same direction as the shorter side of the triangular piece.

* Go ahead and connect the upper base's extrusion to the long side of the triangular piece via a small beam, then use another small beam to connect the end of the servo horn extrustion piece to the shorter side of the main upper beam.

* Proceed to connect your final small beam from the small side of the triangular piece to the upper part of the claw platform and connect tbe long end of the main upper beam to the lower part of the claw platform

* Finally, just assemble the claw section by inserting the micro servo, screwing in its shortened servo horn with its claw pinchers and gears. 

(Also, don't forget to tape in your color sensor onto the front of the mirco servo and wire up all your connections with your thumb sticks if you have them)


(Figure 6: Top picture of finished arm)


(Figure 7: Side picture of finished arm)


(Figure 8: Front picture of finished arm)


(Figure 9: Back picture of finished arm
