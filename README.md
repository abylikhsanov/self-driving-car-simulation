# Self Driving Car Simulation
Using the simulator to gather the data (images) and using Deep Neural Network to train, validate and test a model with Keras. The model will output a steering angle to an autonomous vehicle.

The final simulation result is 

The simulator can be obtained here (Linux):
https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f0f7_simulator-linux/simulator-linux.zip

(macOS):
https://d17h27t6h515a5.cloudfront.net/topher/2016/November/5831f290_simulator-macos/simulator-macos.zip
# Required options

  ```sh
$ Keras==1.2.1
$ numpy==1.13.1
$ matplotlib==2.0.2
$ ipython==6.1.0
$ pandas==0.20.3
$ tensorflow==0.12.1
```




## Installation

This simulation required Python 3 in order to run and options (libraries) above.


```sh
$ cd self-driving-car
$ python drive.py model.h5
```

This will create a model that will make a car drive autonomously. 
In order to produce a video, you can use, video.py file:
```sh
$ python video.py run1
```
Creates a video based on images found in the run1 directory. The name of the video will be the name of the directory followed by '.mp4', so, in this case the video will be run1.mp4.

Optionally, one can specify the FPS (frames per second) of the video:
```sh
$ python video.py run1 --fps 48 
```
Will run the video at 48 FPS. The default FPS is 60.

