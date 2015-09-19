# MotionDetection
A quick program that I put over the weekend to detect movement of arm to flip through slides and images.

#Things you need.
* [OpenCV](http://opencv.org/)
* [numpy](http://www.numpy.org/)
* [PyUserInput](https://github.com/SavinaRoja/PyUserInput)

#How it works

The program uses webcam to capture images, and finds the absolute difference between 3 consecutive images. It uses this information to check whether any motion is happening. If the movement goes beyond a certain threshold (Currently set by trial and error) it checks whether the movement was from right to left or left to right. It emulates the corresponding key tap so that this works across applications. It is a very rudimentary technique that uses no scientific measure, but hey, it works!


#To Do
* Deal with blank frame issue on Windows
* Make it truly cross platform
 
#Special Thanks to 
* [Paul Barton](https://github.com/SavinaRoja) Author of PyUserInput
* [Matthias Stein](http://www.steinm.com/#About)
 - Whose tutorial I shamelessly rippedoff to the point I'd understand. 