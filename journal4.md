# *My 4th Info Science Journal Entry | Feb 20th 2020*

1. **What did we do?**

We were given a piece of paper and with it, write down instructions to create a chess pattern on Processing. This took many trials and fails and confusion, but by the end of class, I did it! I also played around with the position and colors of the squares for awhile, just to explore its exact functions. 

```
Big Problem: Create a Chess Pattern
Sub-Problems [and solutions]: 
 - create a square          [square(x,y,size)]
 - fill it black            [fill(0)/stroke(225)]
 - create a horizontal line [line(x,y,x2,y2]
 - repeat things            [for loop]
 - offsetting               [global offset/offset = offset + 1]
   
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

I learned that instead of repeating the same code but with slight adjustments, we could instead just use 'for loop'. It was quite a hard code, but eventually I understood it. I also learned about the exact functions of x and y and using offset, which is a new concept for me. 

```
global offset
offset = 50

def mouseClicked():
    global offset
    offset = offset + 1
    

def setup():
  size(500, 500)
  background (0, 255, 0)
  
def draw(): 
    stroke(0) # lines are black
    y = 50
    for inc in range(9):
        line(0,y,500,y)
        y = y + 50
    
    fill(0)
    stroke(225)
    y = 0
    for rows in range(5):
        x = 0
        for rep in range(5):
            square(x,y,50)
            x = x + 100
        y = y + 100
    y = 50 # start of the even rows
    offset = 50
    for rows in range(5):
        x = 50
        for rep in range(5):
            square(x,y,50)
            x = x + 100
        y = y + 100

```

3. **What questions do I have?**

Q: Where does the term 'global offset' come from and what does it mean exactly? What are some easy-to-code illusions?
A: https://www.101computing.net/optical-illusions/

# Homework

1. Research about optical illusions 
2. Select one optical illusion that is simple enough
3. Try to code the illusion in Processing 

# Solution to the homework 

```
1. My main research places were freecodecamp.org and https://www.101computing.net/optical-illusions/
2. The Kanizsa Triangle
3. 
def setup():
    size(600, 600)
    background(255)
    
def draw():
    fill(0)
    ellipse(100, 100, 100, 100)
    ellipse(400, 100, 100, 100)
    ellipse(250, 400, 100, 100)
    
    strokeWeight(10)
    stroke(0)
    fill(255)
    triangle(250, 50, 100, 300, 400, 300)
    stroke(255)
    fill(255)
    triangle(100, 100, 400, 100, 250, 400)

```
