# Video Streaming Using Webcam in Flask Web Framework

This project demonstrates how to implement real-time video streaming using a webcam within a Flask web application. It captures video frames from the user's webcam and streams them through a web interface in real time. This setup is built using Python, Flask, and OpenCV for capturing and encoding the video feed.

## Features

- **Real-time video streaming**: The webcam feed is streamed live in the browser using Flask and OpenCV.
- **Efficient frame handling**: Frames are captured, encoded, and served with optimized performance.
- **Simple and lightweight**: This project provides a minimal, easy-to-understand implementation, ideal for beginners.

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.x
- Flask (`pip install flask`)
- OpenCV (`pip install opencv-python`)

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/Video-Streaming-Using-Webcam-In-Flask-Web-Framework.git
    cd Video-Streaming-Using-Webcam-In-Flask-Web-Framework
    ```

2. **Install required dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the application**:

    ```bash
    python app.py
    ```

4. **Access the video stream**:

    Open your web browser and navigate to:

    ```
    http://127.0.0.1:5000
    ```




## Code Explanation

1. **Webcam Capture**:
   - The `cv2.VideoCapture(0)` command is used to access the system's webcam.
   
2. **Frame Generation**:
   - Frames are continuously read from the webcam, encoded as JPEGs, and then sent as part of an HTTP response using Flask's `Response` object.

3. **Video Streaming**:
   - The `generate_frames()` function yields frames in a format compatible with HTML5 video streams.
   - The `/video` route serves the video feed, while the `/` route renders the homepage template (`index.html`).

## Example Output

You should see the live video stream from your webcam in the browser.


