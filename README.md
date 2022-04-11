# BeginningPython

name = "George"
#print ("hello,", name + "!")
print ("hello" , name)
print name
print "hello," , name
from math import sqrt
print(sqrt(36))
import math
print(math.sqrt(25))


# draw some triangles

import turtle

turtle.color("green")


myDrawnLines = 0
myLineLength = 80
myAngleSize = 60
while myDrawnLines < 6 :
  turtle.forward(myLineLength)
  turtle.right(myAngleSize)
  myDrawnLines += 1

#draw a closed shape with however many sides you want
myPolygonSideCount = 50
myDrawnLines = 0
myLineLength = 80
myAngleSize = 360/myPolygonSideCount
while myDrawnLines < myPolygonSideCount :
  turtle.forward(myLineLength)
  turtle.left(myAngleSize)
  myDrawnLines += 1
  
  
  
  for char in "hello":
   print(char)

for i in range(2, -10, 4):
  print i
  
import turtle 
#draw a closed shape with however many sides you want
myPolygonSideCount = 3
myDrawnLines = 0
myLineLength = 360/myPolygonSideCount
myAngleSize = 360/myPolygonSideCount
while myDrawnLines < myPolygonSideCount :
  turtle.forward(myLineLength)
  turtle.left(myAngleSize)
  myDrawnLines += 1
  
  
for hi in range(5):
  print(hi)
  
print("-"*10)

for lo in range(7, -7, -3):
  print(lo)
  
print("-"*10)
  
phrase = "Monty Python"
for letter in phrase:
  print(letter, end="-")
print()
  
print("END")

import turtle
turtle.color("orange")

size = 100
for sides in range(0,3,1):
  turtle.forward(size)
  turtle.left(120)
  
  
  
  
  def add(x, y):
  print("I will add the numbers %d and %d" % (x, y))
  return x + y

sum = add(5, 7)
print ("=", sum)
  
  
  ----
  
  
  import turtle 
turtle.color("green")


def back(space):
  turtle.penup()
  turtle.backward(space)
  #turtle.forward(space)
  #turtle.down()
  turtle.pendown()

def polygon(sides):
  #draw a closed shape with however many sides you want
  myPolygonSideCount = sides
  myDrawnLines = 0
  myLineLength = 360/myPolygonSideCount
  myAngleSize = myLineLength
  while myDrawnLines < myPolygonSideCount :
    turtle.forward(myLineLength)
    turtle.left(myAngleSize)
    myDrawnLines += 1
    
polygon(3)
back(60)
polygon(4)
polygon(20)
  
FROM TRINKET

  import numpy
import matplotlib.pyplot

# Load data
data = numpy.loadtxt(fname='inflammation-01.csv', delimiter=',')
# Make Figure
fig = matplotlib.pyplot.figure(figsize=(5.0, 7.0))

# Create subplots in 3 rows and 1 column
axes1 = fig.add_subplot(3, 1, 1)
axes2 = fig.add_subplot(3, 1, 2)
axes3 = fig.add_subplot(3, 1, 3)

# Plot and label the average, max, and min of the data
axes1.set_ylabel('average')
axes1.plot(data.mean(axis=0))

axes2.set_ylabel('max')
axes2.plot(data.max(axis=0))

axes3.set_ylabel('min')
axes3.plot(data.min(axis=0))

fig.tight_layout()

matplotlib.pyplot.savefig("plot.png")

# Code adapted from Software Carpentry. Check out the full lesson here:
# http://swcarpentry.github.io/python-novice-inflammation/01-numpy.html
