# vismem_toolbox
Functions for creating visual memory experiments

This is a js file I made for creating visual memory experiments with basic shapes in canvas. I worked on this one weekend because: 

1. I found chipmunk js to be too complex
2. I hadn't learned how to use jquery yet (which would've made all this much, much prettier)

Essentially it stores shapes in an array. Many of the shapes have proprties like orientation, color, etc. You use make[SHAPE] functions to add shapes to the objects array and then input the objects array along with the specified canvas to the drawObjects() function. By default, new shapes are stored in an array called objects. But you can also manually specify what array you want to store them in.

Creating a circle with radius 25 at (10,100) would go something like this:

current_objects[0]=makeCircle('test_circle1',10,100,25)
drawObjects(canvas_context,current_objects)

Other useful functions:

1. checkOverlap(current_objects)-Checks if the shapes in current_objects overlap
2. erase(canvas_context)-Remove all drawn shapes

You can see what you can really do with this js file at http://www.evullab.org/ksDissDash/
