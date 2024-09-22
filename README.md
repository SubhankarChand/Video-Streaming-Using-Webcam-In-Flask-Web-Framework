# Video Streaming Using Webcam in Flask Web Framework

This project demonstrates a simple and effective way to implement real-time video streaming using a webcam within a Flask web application. By leveraging Python, Flask, and OpenCV, the application captures video from your webcam and streams it directly through a web interface in real time.

## Features

- **Real-time video streaming**: Live webcam feed streamed directly to a web browser using Flask.
- **Optimized performance**: Efficient frame handling with OpenCV for smooth video output.
- **Lightweight and simple**: Minimalistic code, ideal for beginners and easy to integrate with other projects.

## Prerequisites

To run this project, ensure you have the following installed:

- Python 3.x
- Flask (`pip install flask`)
- OpenCV (`pip install opencv-python`)

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/SubhankarChand/Video-Streaming-Using-Webcam-In-Flask-Web-Framework.git
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
   - The `cv2.VideoCapture(0)` command accesses the system's webcam.
   
2. **Frame Generation**:
   - The `generate_frames()` function reads frames from the webcam, encodes them as JPEGs, and streams them using Flask’s `Response` object.
   
3. **Video Streaming**:
   - The `/video` route streams the video feed using a multipart HTTP response, while the `/` route renders the homepage (`index.html`).

## Example Output

When you access the web application, you will see the live video feed from your webcam in your browser.

## Contributing

Contributions are welcome! If you'd like to improve this project, feel free to submit a pull request.



### Author

Developed by [Subhankar Chand](https://github.com/SubhankarChand).



