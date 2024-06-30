# ATControlROV
This application enables the determination of optimal values for controlling the attitude of the ROV BlueROV2 and BlueROV2 Heavy through a series of controlled trials and data processing. It facilitates both advanced and novice users in understanding and adjusting the ROV control system.

The application utilizes various MATLAB tools and Python libraries to establish communication and control of the ROV.

Tools and Libraries Used:

MATLAB:

•	Control System Toolbox

•	Signal Processing Toolbox

•	System Identification Toolbox

Python libraries:

•	Pymavlink

•	pymavlink.quaternion

•	sys, os, math, pathlib and time 

Application Description:

The main application is named BlueROV2.mlapp or BlueROV2Heavy.mlapp depending on the ROV model. The user interface allows for conducting trials in segments through a series of buttons. This setup enables advanced users to directly access the necessary options and novice users to understand each part of the ROV control system.

Recommended Procedure:

1.	Set Test Parameters: Enter the values for Roll, Yaw, Pitch, and Depth, then press "Set Test Parameters".

2.	Reset PID: Press "PID0" to set the ROV PID values to zero.

3.	Conduct Trials and Process Data:

4.	Yaw:
 
    4.1.	Press "YAW", process data, and adjust PID Inner Loop. 

    4.2.	Press "YAW2", process data2, adjust PID Outer Loop.

    4.3.	Press "Save Yaw Results" to test the movement with the calculated PID values and save the results in the "results" folder.
5.	Roll: 

    5.1.	Press "ROLL", process data, and adjust PID Inner Loop. 

    5.2.	Press "ROLL2", process data2, adjust PID Outer Loop.

    5.3.	Press "Save Roll Results" to test the movement with the calculated PID values and save the results in the "results" folder.

6.	Pitch: 

    6.1.	Press "PITCH", process data, and adjust PID Inner Loop.

    6.2.	Press "PITCH2", process data2, adjust PID Outer Loop.

    6.3.	Press "Save Pitch Results" to test the movement with the calculated PID values and save the results in the "results" folder.


Restrictions and Recommendations:

•	It is recommended not to change the target values or test duration, although advanced users may modify these values according to their specific needs.

•	Execution Order: Follow the recommended order to ensure proper control loop configuration.

•	After executing the movement tests, the vehicle's internal state is reset to avoid errors in the next test run. Please wait before continuing with the next test.
