The program returns a value that seems random between 1m and -1m. Even though the result seems random the cause isn't. 
The reason it isnt zero is because the value gets overwritten. 
When one thread reads a value and before sending it to the ALU another thread updates it, it will do the calculations based on the old values. 
This will result in a diviation from the decired value.
