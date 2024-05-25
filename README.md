This is a repo made specifically for the Mech Tech Dragons 422 FRC Robotics Team, but anyone can use it!
Essentially, we are using the Mindstorms software and their "Hub To Hub" Coding blocks to establish a bluetooth connection between two spike prime bricks
We want to use this connection to make an RC Car

First, download both transmitter1 and reciever 1.
Your transmitter device should use a Touch sensor connected to port C and a motor of any kind connected to port A of the Spike Prime.
Below is a picture of the type of controller we are trying to emulate with the Spike Prime Brick:
![rc](https://github.com/nihalpothunoori/SpikePrime-RC-Car/assets/63886532/8614fbea-024a-4959-8c2f-cd11c9e41ecc)

Next make a simple tank (car with ONLY TWO WHEELS/MOTORS), with the movement motors being ports A and B. (If the car is going backwards when you press the touch sensor/trigger, just swap the wiring.)

You are done with the hardware.

For the software, we will need to downgrade the software on the hubs so that we can run the Mindstorms software on them.
Go to this tool on Google Chrome and follow the instructions to erase the Spike Prime Software and install the Legacy Software. You know the Legacy Software is installed when there is a white circle instead of a green circle.

https://spikelegacy.legoeducation.com/hubdowngrade/#step-1

Note: you will need to connect these Spike Prime Bricks back to the official Spike Prime software and upgrade them to newest Spike Prime Version (Green circle instead of white circle) if you want to use the actual official Spike Prime Code Editor and not the Mindstorms Editor.

After that, open up both code files on the Mindstorms software.
Connect your Spike Prime Bricks and let the new Mindstorms software download.

If you are only making one pair of reciever and transmitter, you will not need to edit the code. You can just upload the correct code to each brick respectively and it should work. Enjoy!

If you want to make multiple reciever/transmitter pairs, you will need to read the comments in the code.
The way these bluetooth connections work is via the signal name.
So if you have two cars whose code is telling them to look for a signal named "forward1", then only one of the cars will recieve that signal and be responsive. The other will not recieve the signal.
So if we want multiple pairs, we need to change the name of the signals that new transmitters/recievers work with.

I've included three different signals in my code, but its fairly easy to make new pairs: click on the green "hub transmit signal" drop down and select "make a new signal".

Email npothunoori@gmail.com for any questions!
