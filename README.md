Real-Time Hand Distance Measurement Using OpenCV and MediaPipe
I developed a real-time hand distance measurement system using OpenCV and MediaPipe. The goal of this project is to estimate the distance of a hand from the webcam based on its apparent size in the captured frames.

How It Works
The system utilizes MediaPipe’s hand tracking model to detect a hand in the video feed and determine its bounding box dimensions. By using a simple camera calibration technique, I estimate the distance of the hand from the webcam based on the perceived width of the detected hand. The calculation follows the formula:

Distance = (Known Width * Focal Length) / Perceived Width

where:

Known Width is the average width of a human hand (set to 8 cm).
Focal Length is a predefined constant that requires calibration (set to 500 for initial testing).
Perceived Width is the width of the detected hand in pixels.
Features

✅ Real-time Hand Tracking – Uses MediaPipe to detect and track hands dynamically.

✅ Bounding Box Detection – Draws a rectangle around the detected hand.

✅ Distance Estimation – Computes and displays the estimated distance in centimeters.

✅ Live Video Feed – Captures and processes frames continuously.

✅ User-Friendly Exit – Press 'q' to exit the program smoothly.


Applications

This project can serve as a foundation for gesture-based interactions, AR/VR applications, and human-computer interaction systems. With further calibration and improvements, it can be extended for use in robotics, accessibility tools, and touchless interfaces.

Next Steps

Improve distance accuracy with better focal length calibration.
Extend the model to detect multiple hands and compute distances separately.
Implement depth estimation techniques for enhanced precision.
This project was a great opportunity to explore computer vision and real-time processing, and I’m excited to expand on it further! 🚀
