# Creating-an-Autonomous-Car-Using-Deep-Learning-with-Python
Complete Guide to Self-Driving Car with Udacity's Car Simulator Environment and Deep Neural Networks
### Understanding Behavioral Cloning

Behavioral cloning is a technique used in autonomous vehicle systems. In this approach, instances where a human or an expert takes control of the vehicle and guides it to perform a specific task are recorded. Later, these recorded data are used to train an artificial intelligence model. This model attempts to mimic the movements and decisions made by the human or expert. As a result, autonomous vehicles can exhibit human-like behaviors and accomplish specific tasks using this model.
<div align="center">
  <img src="images/Resim58.PNG" alt="Imitation Learning">
  <p><em>Imitation Learning</em></p>
</div>

### Driving Simulator: Udacity
Udacity's autonomous vehicle simulator offers students the opportunity to develop autonomous vehicle software. It provides an environment that mimics real-world scenarios, allowing students to practice, debug, and enhance their skills. This simulator provides students with real-world experience while reducing costs and risks.

The simulator includes two tracks. One is considered simple, while the other is more complex. Here, "simple" implies tracks with fewer curves and easier driving. The simulator has two modes for driving: (1) Training mode and (2) Autonomous mode. The Training mode offers the option to record your driving and capture training datasets.
<div align="center">
  <div style="display: inline-block; margin-right: 10px;">
    <img src="images/Resim61.PNG" alt="Result1" width="400">
    <p><em>Basic track</em></p>
  </div>
  <div style="display: inline-block;">
    <img src="images/Resim62.PNG" alt="Result2" width="400">
    <p><em>Complex track</em></p>
  </div>
</div>

## Data Collection

To initiate the process, an autonomous vehicle simulator is used. This simulator, provided from a source like Udacity, enables driving a virtual vehicle on predetermined tracks to generate training data. The simulator's capability to create your own visual dataset facilitates working on the problem. Some reasons why this feature is beneficial include:

- The simulator simulates driving features such as having three cameras on the car. These three cameras are situated in the center, right, and left of the car's front, and continuously capture images during recording in training mode.
  
- Image flow is captured, and the location on the disk where the data will be saved can be set after pressing the record button. Image sets are sophisticatedly labeled with center, left, or right appendages denoting from which camera the image was captured.
  
In addition to the image dataset, it also creates a datalog.csv file. This file includes the current path of the image and relevant steering angle, throttle, brakes, and car speed at that moment.

