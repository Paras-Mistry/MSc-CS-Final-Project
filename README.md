# Live face detection

# Steps to perform the code

1. Install OpenCV library: You will need to install the OpenCV library to perform the face detection. You can install it using pip by running the command pip install opencv-python.

2. Download the haarcascade classifier files: You will also need to download the haarcascade classifier files, which are used to detect faces in the image. You can download the haarcascade_frontalface_default.xml file from the internet.

3. Create a new Python file and import the required libraries: Create a new Python file in your project and import the OpenCV library and other required libraries such as numpy.

4. Load the cascade classifier: In the Python file, load the cascade classifier using the cv2.CascadeClassifier() function and passing the path of the haarcascade_frontalface_default.xml file as the argument.

5. Open the webcam: Next, open the webcam using the cv2.VideoCapture() function and passing the value 0 as the argument. This will open the default camera on your device.

6. Start a loop to capture frames: Use a while loop to continuously capture frames from the webcam. Inside the loop, use the read() function to capture a frame from the webcam.

7. Convert the frame to grayscale: Convert the captured frame to grayscale using the cv2.cvtColor() function.

8. Detect faces in the frame: Use the detectMultiScale() function of the cascade classifier to detect faces in the grayscale frame. This function returns an array of coordinates of the detected faces.

9. Draw rectangles around the detected faces: Use the cv2.rectangle() function to draw rectangles around the detected faces.

10. Display the output: Use the cv2.imshow() function to display the output with the rectangles drawn around the detected faces.

11. Release the webcam: Release the webcam and close all open windows using the cv2.VideoCapture.release() and cv2.destroyAllWindows() functions.
