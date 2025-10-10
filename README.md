**Overview**

The Real-Time Lane Detection and Tracking System for Autonomous Vehicle Navigation Using Computer Vision is an implementation of a computer vision–based framework capable of detecting and tracking road lane boundaries in real time.
The system processes live or recorded driving footage to identify lane markings and visualize them on the road scene, forming a foundational component for autonomous driving and advanced driver-assistance systems (ADAS).

The repository contains a complete pipeline built using Python and OpenCV, demonstrating practical, efficient, and reliable lane detection using classical image-processing methods.

**Objectives**

To develop a robust real-time lane detection system based on computer vision techniques.

To provide accurate and stable lane tracking under varying environmental and lighting conditions.

To create a modular and extensible framework suitable for integration into autonomous navigation systems.

To demonstrate the practical application of OpenCV in road perception tasks.

**Features**

Real-Time Detection: Processes live video streams or prerecorded footage seamlessly.

Edge-Based Lane Identification: Uses Canny edge detection for boundary extraction.

Region of Interest (ROI) Filtering: Focuses analysis on relevant road areas to improve performance.

Line Detection and Tracking: Implements the Hough Transform to identify and track lane lines.

Visual Overlay: Draws detected lane boundaries on the original frame for clear visual representation.

Scalable Framework: Can be enhanced with deep learning–based segmentation models for greater robustness.

**System Workflow**

Frame Capture
The system reads frames from a camera or video file.

Preprocessing
Each frame is converted to grayscale, blurred using a Gaussian filter, and processed with the Canny edge detector to highlight potential lane boundaries.

Region of Interest (ROI)
A polygonal mask is applied to limit detection to the roadway, filtering out unnecessary regions.

Lane Detection
The Hough Line Transform identifies linear features corresponding to lane markings.

Visualization
Detected lanes are drawn over the original frame to provide a real-time view of the driving lane structure.

**Requirements**

Python 3.x

OpenCV

NumPy

(Optional) Matplotlib for visualization

Install the dependencies with:

pip install -r requirements.txt


**Running the Project**

**Clone the Repository**

git clone https://github.com/yourusername/Real-Time-Lane-Detection-and-Tracking-System-for-Autonomous-Vehicle-Navigation-Using-Computer-Vision.git
cd Real-Time-Lane-Detection-and-Tracking-System-for-Autonomous-Vehicle-Navigation-Using-Computer-Vision


**Execute the Main Notebook or Script**

If running the Jupyter notebook version:

jupyter notebook X_Lane_Detection.html


Or if using a converted Python script:

python X_Lane_Detection.py


**To Process a Custom Video**

python X_Lane_Detection.py --input path/to/video.mp4


**Output**

The system displays the processed video feed with detected lane lines overlaid on the original frames.
This visualization effectively demonstrates the lane perception capability required for autonomous vehicle navigation.

**Future Enhancements**

Integration of deep learning–based segmentation networks (e.g., U-Net, SegNet).

Implementation of lane curvature estimation and vehicle path prediction.

Development of a lane-departure warning and driver-assistance interface.

Optimization for night driving, wet roads, and complex lane geometries.
