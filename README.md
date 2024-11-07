Here's a Python script that demonstrates a simple application for person of interest localization using OpenCV and face recognition.

In this script, we use OpenCV's VideoCapture to access the default webcam. 
We then load the image of the person of interest and encode it using the face_recognition library.
We create arrays to store the known face encodings and their corresponding names.

In the main loop, we read frames from the video capture, resize them to 1/4 size for faster processing, and convert the color from BGR to RGB. 
We use face_recognition to find all the faces in the frame and their corresponding encodings.

For each detected face, we compare it with the known faces using the compare_faces function. 
If a match is found, we retrieve the name of the person of interest. 
We draw a rectangle around the face and label it with the name using OpenCV's drawing functions.

Finally, we display the resulting image and wait for the 'q' key to be pressed to quit the application.

Note: Make sure you have the required libraries installed (opencv-python, face_recognition) and replace "poi.jpg" with the path to your image file.
