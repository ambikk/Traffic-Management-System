# Traffic-Management-System
With ever increasing traffic in the country, this project is here to control the traffic with the help of a smart traffic system using IoT, Data Analysis and Computer Vision.
Contains camera side code in cannyedge.py. the server files are present in tms directory the codes for Arduino and wiznet are present in a Text file
## Story
Living in Bangalore, India, you have to deal with hustle and bustle of the city. This city never sleeps and its road are always packed. We, the students of Faculty of Engineering, Christ (Deemed to be University), Bangalore, seek to mitigate this problem with the help of data analysis and IoT solutions.

The biggest question in any project is to how to go about the implementation of an idea. We came across a library called OpenCV, this tool helps us in extracting density of traffic at any point of time. Edge Detection is one way to go about this idea, we use Canny Edge Detection to detect edges. Here is how Edge Detection works.

![1](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/1.jpeg)

![2](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/2.jpeg)

After performing Edge detection we calculate the means of each image processed by the algorithm using the mean of the reference image, in this case the reference image is an image when there is no traffic using this image we can then compare images generated in real time and teach the computer what high low traffic looks like. We should really be careful when we are selecting these images.

The image above displays the image processed by Canny Edge Detection.

# Some Detail on the Components Used
For the server, I used Python's framework called Django. For installation tutorials, please refer the following link:
https://www.youtube.com/watch?v=qgGIqRFvFFk&t=6s&ab_channel=thenewboston

For the MQTT part, I have used Paho on the server side.

Client side, you need to import an MQTT library you can get that by searching for it on

Now, how does everything fall in place? The following image illustrates how all the components fall in to place.

![3](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/3.jpeg)

A view of the login screen:

![4](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/4.jpeg)

A view of the main screen:

![5](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/5.jpeg)

This image gives us the comparison of traffic we are dealing with at each junction.

A view of the API:

![6](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/6.jpeg)

The API helps to transfer data from the camera to the server.

Note: The red board is a WIZ750SR and the blue board is an Arduino Uno.

Too complex to understand? Do not worry! We have made a video.

https://www.youtube.com/watch?v=58E0J_TiXaQ&ab_channel=DYLANPHILIPJOSE1660333

Step 1: Connect a RS232 cable to your Wiznet evaluation board.

Step 2:Take a pair of jumper wires

Step 3:Connect one jumper wire to pinout number 2 and one jumper wire to pinout number 5

![7](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/7.png)

The diagram above will help you with the connections.

Step 3: Take the jumper wire connected to pin 5 and connect it to the GND in your Arduino

Step 4:Take the jumper wire connected to pin number 2 connect it to the RX or 0 digital

![8](https://github.com/ambikk/Traffic-Management-System/blob/main/readme%20images/8.jpeg)

For the signal connections make sure to connect the lights for junctions A and C in parallel and B and D parallel as well.

## Steps to Upload Code to Arduino
1) Select the 'Arduino Uno' board from the Board manager

2)Select right com port for your device

3) Then upload the code

4) While uploading the code make sure the TX and RX pins are not connected

## Steps to Upload Code to the WIZnet Board
1)Compile the Code from Mbed OS

2) Use the ISP toolkit to upload the code to board

3) Before doing that set the boot switch on your board while uploading

4)After uploading reset the boot switch

5)Test your board with AT commands

## Future Advancements
Our project The Nextraf is not just a mere project that a group of students came up one fine day. It was an idea that was incubated in our minds and after research of over a couple of months we had a clear cut idea of what to do. We were adamant on using our knowledge to contribute to the well being of the society. Hence we have put our heart ,mind and soul in whatever we did and whatever we are going to do ...and what we are willing to do in the future as part of the advancements are the following :

1) Ambulance Detection: Ambulances or rather our life savers find it really difficult to commute through traffic even on highly risky situations. Hence we are here to propose that we are planning to put this away once and for all by enabling the Ambulance Detection feature which we are working on. We will be rolling this out in the future once its perfected and confirmed to be flawless.

2) Driver Behaviour Tracking : With the advent of Machine Learning we thought of why not use the same to track the behaviour of the driver and classify based on rash driving , drunken driving etc helping the authorities maintain a clear record of the drivers starting right from their DL number to their driving history and records.


