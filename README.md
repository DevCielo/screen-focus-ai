# Screen Focus Tracker

A focus tracking tool developed as part of a personal project. This system leverages advanced computer vision and machine learning techniques to measure focus based on eye and face orientation and is calibrated to work based on each individuals screen and camera setup.  

## About

I built this project for a larger personal project I'm working on but due to the significant effort in calculations and finding the right values for various parameters I decided to share this project. It incorporates several advanced technologies and concepts to achieve precise iris tracking and focus calculation.  Adjustments to parameters may be needed depending on screen size, camera angle, and lighting conditions for optimal performance. While it works well in most cases, it is not perfect. For example, tilting the head from right to left can cause minor inaccuracies in focus measurements, though it's not a drastic issue. 

## Features

- **Real-Time Iris Tracking**: Detects and tracks iris position relative to the eye region.
- **Focus Measurement**: Calculates focus percentage based on iris position and head orientation.
- **Head Pose Estimation**: Uses face landmarks to estimate pitch, yaw, and roll of the head.
- **Smoothened Focus Scores**: Implements buffers to smooth out fluctuations in focus calculations.

## Technologies Used

- **OpenCV**: For video capture and image processing.
- **MediaPipe Face Mesh**: To extract facial landmarks with high accuracy.
- **NumPy**: For mathematical operations and vector calculations.
- **Deque**: To smooth out noisy data and create a buffer for metrics.

## Known Issues

- **Head Tilt Sensitivity**: The focus calculation may become slightly less accurate when tilting the head side to side. This is a minor issue that does not significantly impact usability.
- **General Tuning**: The parameters used for focus computation required extensive experimentation. While the current values work well, they may not be universally optimal.

## Usage

To run the project:

1. Clone the repository:
   ```bash
   git clone https://github.com/DevCielo/screen-focus-ai
2. MAY CHANGE DEPENDING ON DEVICE
   ```bash 
   python -m venv venv
   source venv/bin/activate
3. Make sure the ipynb file is connected to the environment and run

## Future Plans
- I plan to add documentation explaining all the code in the future

  
