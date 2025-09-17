# Lab02-Memory

Memory machinations and madness

# Makefile requirement

The make file should support the following targets:

`make compile`

`make run`

`make clean`


### Steps:

    (Print the bullet point number, then print what it tells yout to print)
    
    1. Declare and initialize variables c,i,li of types char, int, and long. Print out the addresses of each variable in hex and decimal.
        What do you notice anything about the addresses?
        Print this question: What do you notice when you run the program more than once?
    2. Declare and initialize pointers for each of your variables pc, pi, pli . Print out the value of what each of the pointers are referencing. (this should be the same value from step 1.).
    3. Use the pointers to modify the values of the original variables and print out the new values.
    4. Declare and initialize an unsigned int variable `ui` and 2 pointers that point to it, one should be an int* and the other should be a char *. Print out the value of each pointer (this should be the memory address), and de-reference each pointer to print out the value each points to.
        
    5. Print out your unsigned int in decimal and hex.
        The printf formatting character for a hexadecimal int is: %x
        The printf formatting character for an unsigned int is: %u
    6. Use the char* to print out each individual byte of your unsigned int.
        The printf formatting character for a single byte in hex is %hhu for unsigned decimal integer and hhx for an unsigned hex, (that is half of half of an integer).
    7. Super helpful option: Try setting the value of your unsigned int to: 1 + 2 + 4 + 256 + 512 + 1024 and then print out the bytes again.
    8. Use the char* to increment each byte of the unsigned int by 1. Print out the unsigned int in both hex and decimal after each modification. When done, print out each byte like in step 9. You may need to reset the char * so that it points to the unsigned int, depending on how you wrote step 4 out.
    9. Perform the same operation as in step 8, except add 16 to each byte.

    10. As you go through this, look at what's happening to each byte, and think about the level of control you have over the memory space used by your program.
    Print an answer to "What values did you see for each individual byte? Can you make sense of them? Does the order make sense?"
    11. If you want to test things further try doing all the above with different kinds of values: Try an unsigned int with a value greater that 2.1 billion.
    

Sample output:
```
1
c:  0x124124  12402584
i:  0x124124  12402584
li: 0x124124  12402584
they are all the same!
2.
pc:0x124124
pi:0x124124
pli:0x124124
3.
pc: x
i:  12
li: 402
4.
intp: 0x7ffee3dbd938 p points to: 
charp: 0x7ffee3dbd938 p points to:
5.
etc
```


