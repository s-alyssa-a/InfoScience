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

Create a program that prints the years from 1900 to 2000:

```
i = 0

def setup():
    for i in range (1900, 2001, 1):
        print ("The year is "), (i)
        
delay (100)

```

Create a program that prints the conversion for Celsius to Fahrenheit 
from 0 C to 100 C:

```
i = 0


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
x = [100, 200]
y = [100, 250]
h = [False, True]
<i>wid = 220</i>
<i>Co = 0</i>

def setup():
    size(500,605)
    for n in range(20):
        x.append(random(0,500))
        y.append(random(0,500))
        h.append(True)
        
def distance(x1, x2, y1, y2):
    a = (x1 - x2)
    b = (y1 - y2) 
    c = sqrt(a**2 + b**2)
    return c
        
def draw():
    global x,y, <i>wid1, wid2, Co, count</i>
    background(255)
    <i>strokeWeight(2)</i)
    <i>count = </i>
        
    for ind in range(len(x)):
        if h[ind] == True:
            fill(255) # healthy people
        else:
            fill(255, 0, 0) # infected people
            
        circle(x[ind], y[ind], 40)
        for nei in range(len(x)):
            if nei == ind:
                continue
            d = distance(x[ind], x[nei], y[ind], y[nei])
            if d < 40 and (h[hei] == False or h[ind]== False):
                h[ind] = False
                h[nei] = False
      
        
    for m in range(len(x)):
        x[m] += random(-20,20)
        y[m] += random(-20,20)
        if x[m] > 500: x[m] = 500 # kanan
        if y[m] > 500: x[m] = 500 # bawah
        if y[m] > 0: y[m] = 0 # atas
        if x[m] > 0: x[m] = 0 # kiri
    
    delay(50)
   

```

Add a bar graph at the bottom right corner of the screen that counts the number of infected people and the number of healthy people. It should also show the numbers. Add a counter for the number of times the simulation has run, this is the same as counting the number of times the Draw function is run:


```
I added:

def draw():
    global x, y, wid1, wid2, Co, count
    background(255)
    strokeWeight(2)
    count = 0
    for ind in range(len(x))
        if h[i] == False:
            count += 1
            background(255)
            fill(50)
            text("Infected count:", 300, 540)
            text(count, 390, 540)
            
    Co += 1
    fill(50)
    text("simulation count:", 10, 520)
    text(Co, 110, 520)
    fill(255, 0, 0)
    count = count*10
    rect(30, 530, count, 30)
    fill(255)
    wid1 = wid - count
    rect(30, 570, wid1, 30)
    widCount = wid1/10
    fill(50)
    text("Healthy Count:", 300, 580)
    text(widCount, 390, 580)
    
    if h[ind] == True:
            fill(255) #healthy
        else:
            fill(255, 0, 0) #infected
        circle(x[ind], y[ind], 40)
        
    ...

```

<i> TASK 3 </i>
<b> Complete the table below for 5 different simulation where the number of people moving changes</b>

```
Case Number: Number of people moving | Population size | Number of iteration until all the population is infected |


Case Number 1: 3 | 25 | 345


Case Number 2: 6 | 25 | 257


Case Number 3: 9 | 25 | 144


Case Number 4: 12 | 25 | 103


Case Number 5: 15 | 25 | 69
```

What conclusion can you draw from the simulations you run in step 3. Explain.
```
With more people moving, the less iterations would be needed until all of the population to be infected. This shows how fast and effectively a virus can spread when the rate of people infected is high.
```

Propose another table of simulations. Variables we can change include: population size, distance of infection, movement size, number of people moving.
```
Case Number: Number of people moving | Population size | Number of iteration until all the population is infected |

Case Number 1: 3 | 25 | 335 


Case Number 2: 3 | 20 | 270


Case Number 3: 3 | 15 | 268


Case Number 4: 3 | 10 | 135


Case Number 5: 3 | 5 | 72


With an increasingly smaller population size, but a remaining number of people infected moving, the less iterations would be needed until all of the population is infected. 
```


2. **What did you learn?**

I learn that coding is really hard work and pretty time-consuming - so I seeked for help from Sara, Long and Mirko. They were very helpful and Sara even set a time for us to videocall to help each other with this assignment. Even so, I took a long time understanding what was required by the assignment. 
Data-taking, which was what I practiced in Task 3, proved itself to be simple but still required focus.



3. **What questions do I have?**

None yet.
