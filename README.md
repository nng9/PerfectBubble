## Welcome to the PerfectBubble Project Page


![Intubation](https://user-images.githubusercontent.com/30084214/57289199-ecaaf200-7088-11e9-981d-ca7cde9932c4.png)

# Week 1
### Software

Interface piezo-resistor with MBed to light up an LED when pressed.

### Hardware

Interfact the stepper motor with the mBed. We ran into problems getting the stepper motor to move. We probed everywhere and were puzzed as to why the motor driver was not providing the correct current. We probed the mBed and saw that it was correctly providing input commands to the motor driver. After a couple of days, we found out that the motor driver was faulty. We switched it out and were able to get the stepper motor to move. We played around with the software and determined the number of steps that were required in order to turn the motor one whole revolution. 

# Week 2
### Software
Interface with motor driver to be able to move it clockwise, counterclockwise, and stop.

### Hardware

This week we started designing the syringe pump. We researched syringe pumps that are currently on the market and started thinking of designs that would be best for our application. We saw that a lot of syringe pump designs use two linear rods, but we thought that we could build one with just a single linear rod. Nathan began working on 3D models of the pump in SolidWorks. He 3D printed some parts and was able to get working prototype by the end of this week. 

# Week 3
### Software
Interface piezo-resistor with motor driver to rotate one direction when not pressed and one direction when pressed. At the end of this week we got our pressure sensor. This is the pressure sensor that we plan on placing into the syringe so that it can constantly measure the pressure within the cuff. The sensor has tiny connections so we had to ask for assistance from the Detkin lab TAs for how to solder them. We were eventually able to solder the sensor to a breakout board which allowed us to interface with the sensor using a breadboard. However, the breadboard is too big to put into the syringe. It would have been better if we had designed a PCB for the sensor, but since we did not, we decided that we could no longer place our sensor within the syringe. Instead, we decided that we would place our sensor outside of the syringe and then connect it to the syringe via a long tube. 
### Hardware
This week we refined the design for the syringe pump. There were some imperfections with the 3D printed models. The holes were too small and was causing excess friction. We sanded down these holes and greased the rod with WD40. Moreover, some of our parts did not properly fit the syringe, meaning that the part of the syringe pump that is supposed to pull the plunger back was too large and did not work. So after the baseline demo, we decided to remake this part. Rather than 3D print them, we decided to use laser cutting because it is faster and more preceise. 

# Week 4
### Software

Interface MBed with LCD to display the pressure reading, based on this reading, rotate the motor driver (now attached ot the syringe pump) clockwise or counterclockwise to push the syringe in or out. We implemented a basic control algorithm to maintain pressure. Basically, when a button is pressed, the mBed takes the current reading of the pressure sensor. The system will then try to maintain that pressure. If the pressure drops below the set pressure, then it will trigger the syringe pump to push forward and inflate the syringe. If the pressure gets above the set pressure, then the syringe pump will pull backwards and deflate the cuff. 

### Hardware

# Goals


```markdown
Baseline Goals:
- Be able to measure pressure
- Use a stepper motor controller by an MBed to inflate and deflate the balloon
- Implement a control algorithm that responds to changes in pressure and inflates or deflates the cuff to maintain pressure
- Build a good rig for testing

Reach Goals:
- Add a buzzer to the device that gives an alert to the physician when the pressure has fallen out of range
- Have buttons that correspond to manually moving the syringe
- Log data on pressure and send it to a computer via wifi for analysis.

```

