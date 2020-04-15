# *My 6th Info Science Journal Entry | April 20th 2020*

1. **What did we do?**


<i>TASK 1</i>

Create a new file in processing and create a program that prints 100 bears:

```
i = 0

def setup():
    for i in range (101):
        if i == 1:
            print (i), ("bear")
        else:
            print (i), ("bears")
            
delay (1000)

```

Create a program that prints the years from 1900 to 2000

```
i = 0

def setup():
    for i in range (1900, 2001, 1):
        print ("The year is "), (i)
        
delay (100)

```

Create a program that prints the conversion for Celsius to Fahrenheit 
from 0 C to 100 C

```
c = 0
f = 0

def setup():
    global c, f
    for c in range(0, 101, 1):
        print (c), ("C are"), (f), ("F")
        f = 1.8*c + 32
        
delay(100)
```

<i>TASK 2</i>
<b>The simulation for COVID-19</b>

```

```

Add a bar graph at the bottom right corner of the screen that counts the number of infected people and the number of healthy people. It should also show the numbers:
```
<b>I added:</b>

```

Add a counter for the number of times the simulation has run, this is the same as counting the number of times the Draw function is run.

```
<b>I added:</b>

```








2. **What did you learn?**

I learned that the loop variable (for i in range():) is actually changeable and does not affect the code. 



3. **What questions do I have?**

Q: Where does the term 'global offset' come from and what does it mean exactly? What are some easy-to-code illusions?
A: https://www.101computing.net/optical-illusions/


