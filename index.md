## ECE M202A/CS M213A Embedded Systems Final Project
## Customizable Gesture Based Assistive Control System for Personal Computers

### 1. Abstract
A new gesture based embedded system is proposed that acts as an alternative assistive input for personal computers (PCs). The sensor inputs from a web camera and Arduino are collected by a Raspberry Pi, where image recognition and data processing is performed in real time, and corresponding events are sent to the PC wirelessly to realize with minimal delay. This system is a standalone device that consists of the Raspberry Pi, Arduino and a web camera as aforementioned, and includes BLE and Wi-Fi connectivity. On the PC side, users are able to specify the mapping of specific functionalities and keystrokes to the recognized gestures, allowing for customization based on their preferences and common actions. Although similar systems have been implemented before, the novelties in the system proposed are the use of video for gesture input instead of ultrasonic data, the customizability of control tailored to each user, and the portability of the wireless device.

### 2. Introduction and Proposal
As computer usage has increased due to the move to remote learning and
working, methods to improve workflow through human computer interaction can be explored. One method of doing so is to enhance the methods of input for personal computers. For certain tasks, instead of using a conventional mouse and keyboard, which can be performed through a tedious series of clicks or a complicated keyboard shortcut for performing simple tasks, such as controlling music playback or capturing a screenshot. Therefore, this project explores the possibility of using gesture and other sensor-based input methods through the use of a separate embedded companion device. This device should allow for controls of computer functionalities through simple gestures recognized by the camera, which is parsed on device locally and transmitted through a command to the computer. 

The device is composed of four components: the main personal computer, Raspberry Pi, Arduino Nano 33 BLE Sense, and a USB web camera. The following figure below demonstrates the interaction between them:



The Raspberry Pi acts as a central control for the system, and the web camera and Arduino are connected to the Raspberry Pi to feed inputs into it. The Raspberry Pi takes in the continuous video stream of the web camera and sensor data and continuously runs static image recognition with OpenCV. This is done locally to reduce the processing load on the PC and prevent any heavy network usage when unneeded. Sensors on the Arduino are used to assist with the gesture controls, most importantly preventing false positives in triggering of recognition, which can be activated through the detection of a hand with the proximity sensor or a voice activated method, which would require an either an outgoing internet connection to call voice recognition APIs or be performed locally. 

Once a gesture is detected, it performs the specified task previously defined by the user, by default sending a set of keystrokes to the computer, which recognizes the Raspberry Pi as a keyboard input source. Examples of this flow would be to map gestures to perform screenshots, control online presentation slides, mute and unmute video calls, adjust volume, and play, pause, and other actions in regards to multimedia playback. These specific settings are stored on the Raspberry Pi and can be accessed through the PC to adjust them. 

### 3. Prior Works
### 4. Technical Approach and Implemenetation
### 5. Analysis
### 6. Conclusion and Future Works
### 7. Contributions
### 8. References


