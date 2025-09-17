# Lab02-Memory

Memory machinations and madness

# Makefile requirement

The make file should support the following targets:

`make compile`

`make run`

`make clean`


### Steps:
    
    1. Declare and initialize variables c,i,li of types char, int, and long.
    2. Print out the addresses of each variable in hex and decimal.
        What do you notice anything about the addresses?
        What about when you run the program more than once?
    3. Declare and initialize pointers for each of your variables.
    4. Print out the value of what each of the pointers are referencing. (this should be the same value from step 1.).
    5. Use the pointers to modify the values of the original variables and print out the new values.
    6. Declare and initialize an unsigned int variable and 2 pointers that point to it, one should be an int* and the other should be a char *
    7. Print out the value of each pointer (this should be the memory address), and de-reference each pointer to print out the value each points to.
        The output should look something like: p: 0x7ffee3dbd938 p points to: 133.
    8. Print out your unsigned int in decimal and hex.
        The printf formatting character for a hexadecimal int is: %x
        The printf formatting character for an unsigned int is: %u
    9. Use the char* to print out each individual byte of your unsigned int.
        The printf formatting character for a single byte in hex is %hhu for unsigned decimal integer and hhx for an unsigned hex, (that is half of half of an integer).
    10. Super helpful option: Try setting the value of your unsigned int to: 1 + 2 + 4 + 256 + 512 + 1024 and then print out the bytes again.
    11. Use the char* to increment each byte of the unsigned int by 1. Print out the unsigned int in both hex and decimal after each modification. When done, print out each byte like in step 9. You may need to reset the char * so that it points to the unsigned int, depending on how you wrote step 4 out.
    12. Perform the same operation as in step 11, except add 16 to each byte.

    13. As you go through this, look at what's happening to each byte, and think about the level of control you have over the memory space used by your program. What values did you see for each individual byte? Can you make sense of them? Does the order make sense?
    If you want to test things further try doing all the above with different kinds of values:
    Try an unsigned int with a value greater that 2.1 billion.
    Try a regular int.




