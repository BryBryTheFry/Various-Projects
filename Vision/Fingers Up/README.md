# Fingers Up
A project with the goal of using OpenCV to convert which fingers a hand is holding up into numbers. <br>
Note: It does not have the goal of detecting how _many_ fingers are up, as a pinky, index, and thumb doesn't really mean "three"

# Libraries
- Mediapipe in order to detect the hand bones
- OpenCV to use camera

# Method
Using Mediapipe, we can detect where the joints of the hand are.  <br>
Then, based on where the tips of the fingers are, we can determine if they are down or up.  <br>
Finally, we assign each finger a value based on some power of 2 and can create a table.  <br>
