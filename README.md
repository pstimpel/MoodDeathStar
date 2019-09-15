# MoodDeathStar
A moodlamp and a Death star once had a one night stand...

## Download Death Star stl
https://pinshape.com/items/30200-3d-printed-star-wars-death-star

## 3D Print the stuff
Using my Prusa I3Mk3 I printed the 2 shells in 0.15mm. The inlays were printed in 0.25mm. I was using filament from https://DasFilament.de. I used silver for the shells, and anthracite for the inlays. The housing for the electronics was printed in "nature", and once I ran out of this filament I was using some silver as well.

## Buy the stuff you need (all Amazon links are non profit links and just examples for the stuff I bought)
1 switch, has to handle 3A or more https://www.amazon.de/gp/product/B012MCQ2QO

1 Arduino Nano 5V https://www.amazon.de/gp/product/B07H2VT2JN/

1m of RGB LEDs, you need around 40 LEDs https://www.amazon.de/gp/product/B01LSF4QDM

1 power adaptor to 5V DC, 3A https://www.amazon.de/gp/product/B07HSPT57Y

1 matching socket jack https://www.amazon.de/gp/product/B009PH1J5Y

1 USB mini extension 200mm https://www.amazon.de/gp/product/B01MUEAAF0

1 tactile button 6mm https://www.amazon.de/gp/product/B07Q1BXV7T/

2 screw terminals 5mm https://www.amazon.de/gp/product/B07K31L4FH

1 resistor 260 Ohm, 1/4 Watt

1 resistor 10 kOhm, 1/4 Watt

1 Potentiometer 4.7kOhm https://www.amazon.de/gp/product/B07MM4GPWC

3 2.54mm pin connectors https://www.amazon.de/gp/product/B06XR8CV8P

1 tripolar remale 2.54mm connector, like from a servo cable

some cable, has to handle 3A

some cable, doesn't have to handle 3A

a small piece of stripboard to mount the tactile button on it

## Create the PCB, or use a service to do so
Creating the PCB yourself is always fun. I was using toner transfer method, and the sponge method to remove copper from the PCB. If you dislike to work with chemicals, just order the PCB. You can find the layout inside the electronics folder. The layout was created using the famous and almighty KICAD (http://kicad-pcb.org/ ).

## Add the electronics to the housing
You need some M3x8mm screws to lock down the pcb, the delock connector, the trigger and the USB. The Tactile button goes a small stripboard piece. Just add two cables around 10cm length each to it, and connect the cables to one of the screw terminals on your main pcb. This while act as a trigger to switch between the different illunmination modes.

## Program your Arduino
Inside the Arduino folder there is an example. Nothing fancy, but maybe a start. The illumination was taken from the many examples they deliver with the FastLED library. I simply added some control for the trigger buttin ad the brightness adjusting potentiometer.

## Create the death star
We work from top to bottom. Add the first five inlayes (1, 2, 3 ,4 ,5) to the top shell - the one without an hole in the middle. In the inlays 6 to 31 add 4 holes using a 10mm drill, kind if a circle shape around the middle hole is our goal. Make sure the holes lines up, so you create kind of 4 channels for the led strips. Now create 4 strips of 10 LED each. Connect 2 strips using 5cm tripolar cable. The + and - cable has to handle 3A. The signal cable does not handle much current. Keep in mind the direction of the data signal. Usually these LED strips work in one direction, only.

    ---> data signal direction --->
    strip 1 --- 3 cable 5cm --- strip 2 --- 3 cable 5cm
    strip 3 --- 3 cable 5cm --- strip 4

Use inlay 6. Add the first pair of connected led strips to holes 1 and 2 - it does not matter if your count holes clockwise or counterclockwise, just stick with your decision. Add second pair of strips to holes 3 and 4. Now add inlay after inlay. After inlay 31 do not forget to add the collar from the death star STLs. Now cut the middle standoff from the botton half of the shell. Cut it so, that you do NOT cut into the mounting point on the bottom. Use some super glue to mount the cut standoff to the collar. Add Inlays 31 to around 10, do not forget to drill 4 holes into each of the inlays, as you did with the first half of the inlays. Once you approach the end of the led strips, use your solder iron again, and connect the the cable of strip 2 to strip 3. 

Drill a hole of 7mm onto the stand, and into the mounting point of the bottom half of your death star. Cut 2 pieces of 40 cm of cable from the 3A capable one, and another piece of 40 cm from your low current cable. Feed the 3 cables from the bottom through the stand, through the mounting hole of the lower death star half into the inner part of the death star. And th left inlays to the bottom half. Use some hot glue to fix them. Now solder the 3 cables to strip 1. Connect the other side of the cable to the servo like connector. 

Run a first test. Working well? Use some super glue to connect both halfs of your death star. Mount the "ball" on top of the stand. Use some super glue to fix it there. Use 2 M3-12mm screws, and mount the top stand to the bottom stand. There are holes you use, just use a longer screw driver and the holes on the bottom of your stand.

Brag with your new illimunated Death star.

Video explaining this project: https://youtu.be/01-m4wZ4NJw
