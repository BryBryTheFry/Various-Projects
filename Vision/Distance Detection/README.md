# OpenCV Distance Detection
This is a project that uses OpenCV and Mediapipe to detect and calculate the distance of a hand from the camera.

# Libraries used
- OpenCV for camera detection
- Mediapipe for hand skeleton detection

# Summary
- Uses OpenCV to grab the camera and take the current frame
- Calculates the hand skeleton using Mediapipe
- Uses an equation to calculate distance

# Equation
- The equation was found using regression
- Data points were gathered by printing the distance between points at various distances
- Accuracy suffers at range due to limited resolution and data points

# Problems and Enhancement
- Has difficulty detecting hand and distance at longer distances
  - Due to the limited resolution of the camera
  - Also few data points gathered at long distances, so equation is less accurate
- Has difficulty detecting rotated hand
  - Due to the chosen points for calculations
  - Can be resolved by regathering data points and using different points on the hand
