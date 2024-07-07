# Gesture-Based-Password-Recovery

## Project Overview

This project implements a hand gesture-based authentication system. The system captures the user's hand gesture using the laptop's webcam, converts it into a tensor, and compares it with saved tensors from the password setup phase. If the captured gesture matches a saved gesture within a specified threshold, the user is authenticated and allowed to change the password.

## Features

1. **Capture Hand Gesture**: The system uses the webcam to capture the user's hand gesture in real-time.
2. **Convert to Tensor**: The captured gesture is converted into a tensor, a multi-dimensional array representing the gesture's features.
3. **Compare with Saved Tensors**: The system compares the tensor of the captured gesture with the tensors saved during the password setup phase.
4. **Authentication**: If the captured gesture matches a saved gesture within a certain threshold, the user is authenticated and allowed to change the password.

## Technologies Used

- **OpenCV**: Used for capturing and processing the video feed from the webcam to detect hand gestures. Provides robust tools for computer vision tasks, making it suitable for capturing and processing hand gestures in real-time.
- **TensorFlow**: Used for converting the captured gesture into a tensor and for comparing it with saved tensors.
- **NumPy**: Essential for handling tensors, which are the primary data structure used for representing hand gestures. Used for handling multi-dimensional arrays, particularly for manipulating tensors.
- **Scikit-learn**: Used for defining and implementing the matching algorithm, allowing for a customizable and efficient comparison of tensors. In this project, it is used for defining the threshold and comparing the tensors to determine if a gesture match is successful.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/Vijayadharshni01/Gesture-Based-Password-Recovery.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Gesture-Based-Password-Recovery
   ```

## Usage

1. **Setup Phase**:
   - Run the setup script to capture and save your hand gestures.
   - The system will guide you through capturing multiple gestures to create a reliable reference.

2. **Authentication Phase**:
   - Run the authentication script.
   - Show your hand gesture to the webcam.
   - The system will compare the captured gesture with the saved gestures and authenticate you if a match is found.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any features, bug fixes, or improvements.


## Acknowledgments

- OpenCV for providing robust tools for computer vision tasks.
- TensorFlow and Keras for facilitating the implementation of deep learning models.
- NumPy for efficient handling of multi-dimensional arrays.
- Scikit-learn for providing powerful machine learning algorithms and tools.
