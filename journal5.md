# *My 5th Info Science Journal Entry | (early) April 2020*

Context: <i>Many countries have implemented several measures to contain the spread of the Covid-19 virus including social distancing, border closings, quarantine. We can use a computer to help us visualize and understand the effectiveness of these strategies.</i>

Inquiry question: <i>What strategy is the most efficient to contain the spread of a virus in a general population?</i>

1. **What did you do?**

I read the article "How your personal computer can help science battle the coronavirus while you sleep" by John D'Anna.<br/>
My main take-away was this: Though at times we may feel powerless with everyone that is going on in this world, we have to realize there are ways we can contribute to help, like volunteering to download this software to help find and contribute data towards our frontliners.<br/>
In my opinion, people should enable access to the resources of their personal computers as tools for research, but only if there are aware of the risks. To do so blindly would cause the same amount of damage if they wouldn't volunteer in the first place, if not more.<br/>
While they are assured that uses extensive security safeguards to ensure the system is protected from hacking and difficult to exploit, it should be noted that it is not 100% foolproof and it might be safe to transfer banking information or other important details on your laptop somewhere else. (Similar to the incident with Zoom, the video-calling software) 

I also watched and followed along videos provided.<br/>
For the task at end of #2, I read a bit about how to add values to lists when using Python.<br/>
When coding, I was wondering why it didn't work, only to realize that it was because of the defining of the x and y values in the beginning, I put in the wrong brackets. Once that was fixed, the rest worked fine.

2. **What did you learn?**

I learned that a simulation is defined as a process of alghorithmic modelling on a computer that's used to predict real life behaviour or outcomes.<br/> 
In this particular simulation, we can use abstraction in computer science to recognize properties like body shape and form are not relevant, but instead represent it by something like a circle.<br/>
Also, we're using the random value again like we did before, for the position of the indiviual.

```
#definition of variables
x = []
y = []

def setup():
    size (500, 500)
    for i in range(10):
        x.append(random(0,600))
        y.append(random(0,600))

def draw():
    global x, y
    background (255)
    strokeWeight (2)
    
    #create individuals
    for i in range(10):
        circle (x[i], y[i], 40)
        x[i] = x[i] + random (-10,10)
        y[i] = y[i] + random (-10,10)
    
        #boundaries conditions
        if x[i]>580:
            x[i]=580
        if y[i]>580:
            y[i]=580
        if x[i]<20:
            x[i]=20
        if y[i]<20:
            y[i]=20
        
    delay(100)

```


3. **What questions do I have?**

I don't understand what Q5 meant as in 'behaviours'?

# Homework

What should be some behaviours (at least 3) that we will need to include in our simulation to be a realistic approximation of the current situation in the world? Explain.

# Solution to the homework 

*not yet found*
