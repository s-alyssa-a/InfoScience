# *My 3rd Info Science Journal Entry | Feb 10th 2020*

1. **What did we do?**

We used the 2D dice from last class and made it able to be randomized.

2. **What did you learn?**

How to randomize different shapes in Phytons and using probability.

```.py

x = 0
shape = 0

def setup():
  size(600, 600)
  background (255)
    
def draw():
    x=0
    
def mouseClicked():
    fill(200)
    rect(150, 100, 300, 300)
    n = random(0,6)
    print(n)
    fill(0)
    if n<1:
        circle(300, 250, 55)
    elif n<2:
        circle(200, 350, 55)
        circle(400, 150, 55)
    elif n<3:
        circle(300, 250, 55)
        circle(200, 350, 55)
        circle(400, 150, 55)
    elif n<4:
        circle(200, 150, 55)
        circle(200, 350, 55)
        circle(400, 150, 55)
        circle(400, 350, 55)
    elif n<5:
        circle(200, 150, 55)
        circle(200, 350, 55)
        circle(300, 250, 55)
        circle(400, 150, 55)
        circle(400, 350, 55)
    elif n<6:
        circle(200, 150, 55)
        circle(200, 350, 55)
        circle(200, 250, 55)
        circle(400, 150, 55)
        circle(400, 250, 55)
        circle(400, 350, 55)

```


3. **What questions do I have?**

None for now! 

# Solution to the in-class coding challenge

We were given a list of probabilities, switched laptops with some people in class and tried to spot the odd probability out. It was very interesting and fun, because we only had 3 tries per group, which made it actually really fun!

```.py

x = 0
shape = 0

def setup():
  size(600, 600)
  background (255)
    
def draw():
    x=0
    
def mouseClicked():
    fill(200)
    rect(150, 100, 300,300)
    n = random(0,550)
    print(n)
    fill(0)
    if 0<=n<=99:
        circle(300, 250, 55)
    elif 100<=n<=199:
        circle(200, 350, 55)
        circle(400, 150, 55)
    elif 200<=n<=299:
        circle(300, 250, 55)
        circle(200, 350, 55)
        circle(400, 150, 55)
    elif 300<=n<=399:
        circle(200, 150, 55)
        circle(200, 350, 55)
        circle(400, 150, 55)
        circle(400, 350, 55)
    elif 400<=n<=449:
        circle(200, 150, 55)
        circle(200, 350, 55)
        circle(300, 250, 55)
        circle(400, 150, 55)
        circle(400, 350, 55)
    elif 450<=n<=549:
        circle(200, 150, 55)
        circle(200, 350, 55)
        circle(200, 250, 55)
        circle(400, 150, 55)
        circle(400, 250, 55)
        circle(400, 350, 55)
    
```

    
