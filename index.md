## Blind Sailing
### The Big Idea
Blind Sailing International has been attempting to create a clean and effective solution for blind individuals who want to sail competitively for some years. For several years now, project teams at Olin have attempted to help this initiative by coding a better solution. This means there is a lot of existing code that is only partially functional. The main goal of our project was to improve the functionality and accessibility of the blind sailing project for anyone who may wish to have access. We decided to accomplish this goal by targeting a few specific features to fix, and then implementing them into a pygame simulation so that people can better understand the tools we have provided, without the hassle of going out and actually attempting to sail. In this way, our blind sailing software can even be used to help teach new users the fundamentals of sailing.

![Image 1](SailingDiagram.png "Sailing Course Diagram")
https://www.youtube.com/watch?v=h2csQ_rdOtE&feature=youtu.be&t=25


### User Instructions (Important!!)
Along with cloning and running our code, there are a few things the user must do in order to gain access to the full functionality of our code. Open up the command terminal in your computer, and paste the following commands into your terminal (using ctr-shift-v). After pasting each one, press enter to run and download the packages.

```
python3 -m pip install -U pygame --user
```

```
pip install pyttsx3
```

```
pip install gTTS
```

Once these are installed, the user should be able to simply clone this repository, run our code, and perform the simulation.


### Implementation

Our code, having pieces that have existed for some years before us, will carry an interesting format. Firstly, the pieces of code we chose to improve of the previous project teams (the text to speech and navigation algorithm) are a subset of a lot of existing classes. We are taking these classes that we have "improved" and using them in a visual demonstration, shown in a pygame. Our code will be structured as the diagram below.

![Image 2](FlowChart.jpeg "Structural Flowchart")

Context as to what each piece of the flowchart means is also provided below:

![Image 3](basic-symbols.jpg "Key for Symbols")

In general terms, our final product is a simulation that allows the user to control the boat. There will be varying conditions, and the user may input a request to any of a list of variables (distance to buoy, bearing to buoy, etc), which will then be relayed to them through text to speech.

A portion of code that highlights the mapping of the key inputs is included below:

```markdown

# Description of KeyPad Inputs

def __init__(self):
        options = {'0':('0 gives all information about the other boat'),
                   '1':('1 gives location of the nearest buoy'),
                   '2':('2 gives speed of the boat in meters per second'),
                   '3':('3 gives bearing of boat'),
                   '4':('4 gives wind direction')
 
```

### Results
Our final product is (will be, still in progress as of right now) a pygame simulation of sailing. The simulation contains (or will, again, still in progress) the ability to control a boat on the water. The user must navigate the course while controlling the bearing of the boat and sail direction, and all the while there is a variable wind speed affecting all of these things. The user also has access to a set of tools very similar to those a blind sailor would have while using the blind sailing software Olin has created out on the water. The following is a picture of our current software. 

![Image 1](SailingDiagram.png "Sailing Course Diagram")


### Software Impact Statement




### Project Evolution

### Credit Where it's Due