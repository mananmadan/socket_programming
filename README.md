add how to go forward with the task and also the things that you learned during
the process.

server_code.py will run on pi will create the socket , bind the socket , reading the commands send it to manually and executing these commands on an arduino.

keyboard_controls.py will run on the base computer and will give the commands to the pi through the socket connection.

now basically what we want to do is to integrate the path planning code instead of the keyboard_controls.py so that the velocity commands that are manually given can be given through the path planning code.

now the keyboard_controls.py consists of basically a function called sendDatatoRaspi which sends the final commands to the pi so we have to reatain just that functions and the commands given by that function is
the forwardBackwardSpeed and the leftRightSpeed.

so we have to remove all the other functions such as decreaseleftRightSpeed --> basically the functions that are written for keyboard_Detection of calculating the velocity and put our path planning code in this
code so that our program can achieve what we were trying to do manually

Tasks to be accomplished to make the final code working:


1> check if the python implementation of the path planning code is working or not.

2> learn about socket programming so to be able to test the code.


3>also some minor changes have to done in the path planning code to use it for differential drive robot.
    --> for this task basically have to figure out the math so that the server percives the command you are sending as the commands of a differential model.

  figure out the maths, already written code will function , now have to integrate the path planning module into the code and then convert the commands as per calculated for the differential drive robot
  and publish it on the socket in sendDatatoRaspi functions

The work to be done till sunday is to create the motor controller for the rover.
-->that is done
