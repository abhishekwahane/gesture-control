# Virtual Mouse

Control Mouse using Hand Gestures

![Gesture Control](https://miro.medium.com/max/2000/1*-wc57H4KMXJXZpeze0eVSQ.gif)

#### Introduction

Gesture control using Computer Vision and webcams may not be as accurate as other sophisticated hardware implementations, but for basic actions like clicking, dragging, swiping, scrolling etc. it is a much cheaper yet effective solution.

Such systems can be deployed at Airport Kiosks, Booking Counters, Ordering placing Kiosks, for touch free interaction with the system thereby maintaining hygiene. 

#### Requirements

  - Opencv | Computer vision library
    ```
    pip install opencv-python
    ```
  - Numpy | Fundamental computation
    ```
    pip install numpy
    ```
  - Pynput | Control user input devices
    ```
    pip install pynput
    ```
  - WX | Python GUI 
    ```
    pip install wxpython
    ```
    
    
#### Exceution

Use pythonw command for the program to be able to gain system screen access.

```
pythonw gesture.py
```
 
#### Implementation

It detects two states:
  - Moving mouse
  - Click
  
If it detects 2 objects of color (yellow, can be configured as per choice), it computed their centroid and mouves the mouse accordingly.

If it detects the 2 objects being very close to each other, it considers as click.
