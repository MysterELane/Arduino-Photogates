# Arduino-Photogates
A project to use photogates with arduino and display that data on the computer using Processing.

The goal of this program is to build an interface to use with various photogates that are sold by commercial education companies.  Step 1 will be using the sparkfun Vernier shield to build the basic software that will Record three sets of a data for a car running down a ramp:   Time through Gate 1, time through Gate 2, and time from Gate 1 to Gate 2.  With those three numbers, students will be able to calculate instantaneous speed through each gate, average speend between the gates, and average acceleration from Gate 1 to Gate 2.  

Photogates all work on the same principle:  An infrared LED is either blocked or unblocked from one side of the gate to the other.  Blocking the light coming from the LED from reaching the infrared sensor on the other side causes the first time to register in the software.  Unblocking the light will register a second time, the difference between these two times. is time A, and can be used to calucate Instantaneous speed at A if the size of the blocking object is known.  

When the second gate is blocked, the total time to transition from Gate A to Gate B can be calculated.  When the second gate is unblocked, the time the second gate was blocked can be calculated.  All the data should now be acuired to be able to calculate Speed Through A, Speed through B, average speed between A and B, as well as average acceleration between A and B. 

The output of these pieces of data should go into a processing Program so that times are visible to the user, rather than using a LCD interface.  This can allow for a great deal of creativity in design of the time reporting interface, as well as logging of data.  
