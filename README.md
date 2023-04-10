# CycleFirst
An image Classification project with an esp32 AI-Thinker and Edge Impulse.
## Introduction
This is an Arduino code for a traffic light designed to give cyclists priority over cars in traffic. This is to motivate people in a city to take bicycles instead of cars, thus there are fewer traffic accidents, less noise and more space in a city (parking lots take up a lot of space)

The traffic light uses the Edge Impulse library to recognize and differentiate cyclists from a situation without a bicycle. When a cyclist is detected, the traffic light will give a green light to cyclists and a red light to cars. When no bicycle is detected, cyclists will get red, and cars will get green.

But feel free to modify the code according to your project! The code is made so that you can easily place your code in the loop function. Just remember to put your Edge Impulse library at the top. 

There is also a Hackster.io project coming from this code, so stay tuned!

## Instructions for use
To use this code, you will need an ESP32 module, along with four LEDs (two green and two red). You must also have the Edge Impulse library installed.

Make sure that you have connected the ESP32 module to the correct pins of the LEDs, this will be discussed in detail soon in the hackster.io project.

After you have connected the ESP32 and connected the LEDs, you can upload the code to the ESP32. Once the code is uploaded and the ESP32 module is connected, you can start using the traffic light.

## Important files
The key files in this repository are:

`CycleFirst_Main.ino`: This is the main code that controls the ESP32 module and lights the LEDs based on the Edge Impulse library.

`Bike_detection_V2_inferencing.h`: This is the library used to detect the bikes. It is important to install and use this library correctly for the traffic light to function correctly. Feel free to create your own library and replace it in the code

## Authors
The basic code is from this github repo: https://github.com/alankrantas/edge-impulse-esp32-cam-image-classification. I have modified this code according to my project. I Added an if-then function to associate an action with a certain image score.

## License
The code in this repository is licensed under the GNU Affero General Public License. Please consult the LICENSE file for more information.
