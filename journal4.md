# *My 4th Info Science Journal Entry | Feb 20th 2020*

1. **What did we do?**

We were given a piece of paper and instructions to create a chess pattern.

```
Big Problem: Create a Chess Pattern
Sub-Problems: 
 - create a square [square(x,y,size)]
 - fill it black [fill(0)/stroke(225)]
 - create a horizontal line [line(x,y,x2,y2]
 - repeat things [for loop]
 - offsetting [global offset/offset = offset + 1]
   
Steps:
1. Setup the screen 500 x 500 
2. Set background to white
3. Draw a horizontal line by using y=50, from x=0 to x=500
4. Make the stroke black.
5. Draw a square and fill it black with white stroke.
6. Repeat it by using loop to create 5 other squares across one horizontal line with 100 pixels space between them.
7. Repeat the squares bu using loop, this time vertically.
8. Add in offset to create the visual illusion.
    
```

2. **What did you learn?**

In alghorithm thinking, you have to be detailed because a supercomputer can only be a supercomputer if you feed it superinstructions. Computational thinking is also not limited to only computer-related skills, but it is a way of thinking that can be applied to all kinds of problem in real life as well.

3. **What questions do I have?**

I only have questions about how to create a shape on Processing, which I will find out the answers to while exploring and doing research on it later.

# Homework

1. Research about optical illusions 
2. Select one optical illusion that is simple enough
3. Try to code the illusion in Processing 

# Solution to the homework 

Here I solved the code challenge to create the first letter of my name by using squares in Processing.

```.py

square(10, 10, 20);
square(30, 10, 20);
square(50, 10, 20);
square(70, 10, 20);

square(10, 30, 20);
square(10, 50, 20);

square(30, 50, 20);
square(50, 50, 20);
square(70, 50, 20);

square(70, 70, 20);

square(70, 90, 20);
square(50, 90, 20);
square(30, 90, 20);
square(10, 90, 20);

```
