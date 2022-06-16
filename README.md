# Air-Canvas-with-ML
Computer vision project implemented with OpenCV with Machine learning using the Mediapipe

Ever wanted to draw your imagination by just waiving your finger in air. In this post we will learn to build an Air Canvas which can draw anything on it by just motion of our hands and noticing the landmark on the hand knuckels. A very beautiful project for resume of machine learning people.
We will be using the computer vision techniques of OpenCV to build this project. The preffered language is python due to its exhaustive libraries and easy to use syntax but understanding the basics it can be implemented in any OpenCV supported language.

Here Hand landmarks detection and tracking is used in order to achieve the objective. <br><br>
<b>The youtube video link with full explanation: </b> https://www.youtube.com/watch?v=T7sjrWc4QEc


# Algorithm

1. Start reading the frames and convert the captured frames to HSV colour space.(Easy for colour detection)
2. Prepare the canvas frame and put the respective ink buttons on it.
3. Adjust the values of teh mediapipe intilization to detect one hand only.
4. Detect teh landmarks by passing the RGB frame to the mediapipe hand detector
5. Detect the landmarks, find the forefinger coordinates and keep storing them in the array for successive frames .(Arrays for drawing points on canvas)
6. Finally draw the points stored in array on the frames and canvas .

Requirements: python3 , numpy , opencv, mediapipe installed on your system.

<img src="https://raw.githubusercontent.com/infoaryan/Air-Canvas-with-ML/master/Screenshot%20from%202022-06-16%2019-57-44.png" width="950" height="400">
