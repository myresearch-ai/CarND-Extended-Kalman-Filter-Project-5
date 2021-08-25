# **CarND-Extended-Kalman-Filter-Project-5** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Overview
---

This project utilizes a **kalman filter** to estimate the state of a moving object of interest with noisy lidar and radar measurements. Successful implementation of the filter requires obtaining RMSE values that are lower than the tolerance outlined in the project rubric: *px, py, vx, vy RMSE should be less than or equal to the values [.11, .11, 0.52, 0.52]*.

This project involves the Term 2 Simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases).

This repository includes two files that can be used to set up and install [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac systems. For windows you can use either Docker, VMware, or even [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. Please see the uWebSocketIO Starter Guide page in the classroom within the EKF Project lesson for the required version and installation scripts.

Once the installation for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF

Implementation Flow Path (Algorithm)
---

The schematic below provides a visual summary and approach to implement the Extended Kalman Filter (EKF). For detailed breakdown of the EKF, several resources exist on the web including udacity's nanodegree.


![KalmanFilter](https://user-images.githubusercontent.com/76077647/130775699-3cb18075-d617-43af-8538-ad572d41e23b.JPG)
**Fig 1**: Algorithm. Illustration taken from udacity's course content.

Important Dependencies
---

* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

Basic Build Instructions
---

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make` 
   * On windows, you may need to run: `cmake .. -G "Unix Makefiles" && make`
4. Run it: `./ExtendedKF `

Code Style
---

Please (do your best to) stick to [Google's C++ style guide](https://google.github.io/styleguide/cppguide.html).

Results & Performance
---

Following the EKF algorithm and guidance based on the illustrated flow path above, implementation in this repository accomplished acceptable RMSE scores for both datasets 1 & 2 of which the former was the only required.


![Capture_1](https://user-images.githubusercontent.com/76077647/130776638-bc92dd36-a5f0-4a2f-9482-c302669ba595.JPG)
**Fig 2**: Showing EKF performance on dataset 1

![Capture_2](https://user-images.githubusercontent.com/76077647/130776696-e83f56e0-5a5f-420e-92fb-2c016bece2e5.JPG)
**Fig 3**: Showing EKF performance on dataset 2

References & Credits
---

* udacity (self driving car nanodegree - extended kalman filter module)
* course peers
