---
layout: default
---

# Split Flap Counter 1-0
Summary project for the Digital Fabrication & Prototyping Fundamentals module

I plan to create a Youtube/Instagram Subcriber Counter. The counter will use a split flap mechanism and was inspired by counters like [Smiirl](https://www.smiirl.com/en/store?gclid=EAIaIQobChMIvvTDg8Ls6gIVlH0rCh0ipgDZEAAYASAAEgKEMfD_BwE) and [FlapIt](https://www.flapit.com/). However due to its complexity, i decided to make the counter with only a basic and simple prototype. When I have succeeded this prototype for my DFAB project, I would built on it and make it do awesome things, like the initial plan; A subscriber counter or some other ideas, like a clock.


## Concept

The old school split flap display is cool and mesmerising to look at. To help build my counter, I will be laser cutting a lot of the split flap mechanics and 3D print the house.


## Items Needed

- ### Flaps
- ### Spool
- ### Wheel
- ### 3D Frame or housing
- ### Electronics:
		- Arduino Uno
		- Half size breadboard 
		- 1 push buttons
		- Stepper motor 28BYJ-48 and ULN2003 driver motor.
		- 6 male to female wire
		- 4 male to male wire.
- ### Hardware
		- 2 M4 hex nuts and screws
		- 3 M4 hex nuts and screws
		- Drill for 


## Laser Cuts:
###Flaps

I begin this project with the flaps first beacuse it is the simplest thing to create. I drew my sketch on Fusion 360 and laser cut on a 3mm acrylic board. Since the flaps are quite thick to be placed on a rotating wheel, I could only place digit number 1 till 0. I followed the dimension of a standard business card as my guide. From here, I could estimate the dimension of other laser cutting parts.

The numbers on the flaps are placed using white sticker labels since this is just a prototype. I feel that engraving would be too time consuming and could not be undone if I want to change the characters on the flaps. The font im using is called Solari. I printed it out on paper and cut out using penknife so I could trace it on my sticker labels like a stencil. The flap layout with text was a bit tricky, but once you understand the concept it's pretty simple. Basically the "front" of each flap pair is a whole number, and the "back" of each flap pair has the bottom of the next number and the top of the previous number. So "1" has the bottom of "2" behind its top flap, and the top of "0" behind its bottom flap.

The laser layout for the text modules looks like this:
![](https://github.com/refrigerated/EP1000/blob/master/docs/images/Flaps%20number%20position.jpeg?raw=true)

###Wheel

This part is very tricky for me to get it right. Every millimeter makes a difference. I made few mistakes of getting the holes for each tiny arms of the flaps too wide and too close to each other. The circular holes for the little arms of its flaps is used using the circular pattern tool on fusion. To make sure that the top and bottom flaps do not align to far apart, make sure between each hole is at most 10mm apart. 

The diameter of the wheel also plays a role on making sure it can turn well. I used 60mm for my diameter. One of the wheel has a shape precisedly cutted out following the shape of my stepper motor on the middle. And my other wheel has a M4 hex cutted right on its middle.

I also made 4 rectangluar cuts for my spool to fit in. With some calculations, I could easily figure where the cuts should be.
![](https://github.com/refrigerated/EP1000/blob/master/docs/images/wheels%20with%20hex%20nut.jpeg?raw=true)
![](https://github.com/refrigerated/EP1000/blob/master/docs/images/left%20side%20of%20wheel%20with%20hex.jpeg?raw=true)
![](https://github.com/refrigerated/EP1000/blob/master/docs/images/insert%20extra%20thing.jpeg?raw=true)

###Spool
I made a simple cuboid spool and used the pressed fit method to join them together. Then, to ease my assembly, I glued them together.


###Plates
Initially I plan to make the housing out of laser cuts, however my design falls short for the whole unit to stand up. I created a new one with laser cutting too after carefully measuring the longest end when the whell is spinning.
![](https://github.com/refrigerated/EP1000/blob/master/docs/images/original%20design%20of%20side%20housing.jpeg?raw=true)

###3D Print
The only part that was 3D printed was the spool extension i used to make the split-flap display hold and hang up. It is made of two parts. One is a hollow rod that fits the shape of the motor shaft. And another was an extension shaft to fit the hole of the wheel. The two parts were then forced fit together with a clamp.
![](https://github.com/refrigerated/EP1000/blob/master/docs/images/3d%20printing.....mp4)

This is the 3D that I design but decided to pass. It would take too much time to print and I wasnt sure if the house dimensions are measured perfectly. I am relieved that I laser cutted the housing instead.


### Arduino wiring and Code
The wiring is quite simple for this project. When I upload the code, I should be able to control the stepper motor forward by pressing the Red button. And stops when I released it. It is programmed this way so that the user may control to display what number he chooses to show. 

Stepper Motor:

ULN2003 Driver motor:


## Results

The result works fine. The mmotor can be controlled smoothly. However, the top flap of number 9 does not drop smoothly. The reason must be because of the tight fitted wheels that were glued together. I also made the mistake of placing the sticker numbers upside down. Thus the counter can only be count downwards.

## Conclusion
 I learnt a lot through this project. It is not good looking as I expected and there were a decent amount of mistakes made in measurements. I now learn that I should lower down of my expectations as there were a lot of trial and errors in my design.

## Design files & Source Code

Include all original design files and source code for your project.

## References

[Button Spit Flap White](https://www.instructables.com/id/Split-Flap-Display/)
[Scottbez Split Flap github](https://github.com/scottbez1/splitflap)
[Weather forecast Split Flap](https://www.instructables.com/id/IoT-Split-flap-Weather-Forecast-Powered-by-XOD/)
