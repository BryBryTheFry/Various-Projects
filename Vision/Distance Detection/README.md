This is a project that uses OpenCV and Mediapipe to detect and calculate the distance of a hand from the camera.

Libraries used:
OpenCV for camera detection
Mediapipe for hand skeleton detection

The program uses OpenCV to first grab the camera and open it before taking a photo from the camera.  It then detects any hands in the photo using Mediapipe and creates the skeletons.  Then, using an equation found through regression, it calculates the distance of the hand from the camera.  
The equation was found by recording the pixel distance from one point on a hand to another point and the actual distance from the camera.  Then, after plotting the points, regression was used to create an equation that could be used to calculate the distance of the hand from the camera.  However, due to the lack of data points at longer distances as well as the inherent inaccuracy due to the resolution of the camera, the reported distance may differ from the actual distance at longer ranges.  This could be fixed with more data points and a higher resolution camera.
There is another issue where if the hand is not facing the camera straight on, the distance may be incorrect.  This is likely due to the hand skeleton points chosen and could be resolved by instead using points on the hand that do not change in distance from the camera's perspective when the hand is rotated.
All in all, the project was interesting and helped me to learn how I could use computer vision and AI to detect a hand and use the skeleton to figure out different things, such as distance.
