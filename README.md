# RepCounterV1
*Introduction*

RepCounter Version 1 is Repitition counter during a workout session. It is a physical prototype that can be use during a workout session. 

*Why build RepCounter?* 

Sometimes, i would get distracted and lost count my repititions. Lost count repititions mean you either redo the whole set or just finish the set by feel. Other than that, after finishing a set you need to open up your clock app on your phone and set a timer for resting which is a hassle for me. To solve this problem, i build RepCounter. It counts your repitition for each set and a timer after finishing your current set. 

*Methodology*

Component list:
- Arduino UNO 
- Ultrasonic Sensor 
- LCD with I2C module 
- wires 
- buzzer 
- push button 
- LED light 
- 4x4 membrane keypad
- 220 ohm resistor 

The brain of this devices is Arduino UNO. 

Three main inputs are: 
- Ultrasonic sensor
- 4x4 membrane keypad
- push button

Three main outputs are: 
- LCD screen
- Buzzer 
- LED light

User can type in number of sets, number of repititions, resting time using 4x4 membrane keypad.
Ultrasonic sensor will sensor an object in front of it which then sends the signal to Arduino UNO to count reps. The object in front of it must pass a certain threshold to be counted as 1 repitition.
The push button will act as a start button after the user type in the numbers.

LCD screen will display the menu and resting time. 
Buzzer will act as an audio indicator if you complete a rep, complete a set and when resting time is done. It will produce a buzz sound. 
LED light  also will act as an visual indicator. It will turn on during your set.
