1. Runtime code in python
2. Refactoring

一
from timeit import default_timer as timer #What does this mean?

start_timer = timer() #Variable holds the start time

#Processing Happens here

end_timer = timer() #Variables holds the end time

run_time = end_timer - start_timer #run time duration
print(“The run time was: %f seconds” % run_time)


二
Unit: A segment of a program that handles a problem’s specific requirement

Refactoring: The act of improving the performance and efficiency of the unit (section of a program) without affecting input and the output of the unit
If a program is simplified to its Input → Processing → Output, then we are trying to optimize the “Processing” section of the program by Refactoring

#What does brute force mean?
