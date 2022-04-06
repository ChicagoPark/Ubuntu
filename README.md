# Ubuntu
Ubuntu Installation

### 1. Delete Ubuntu and Clean the SSD card

```bash
1. Delete Ubuntu & Grub: (main) jimnong.tistory.com/677
                         (reference) https://blog.naver.com/smopy/222128374955
                         
2. Clear the SSD card: https://www.youtube.com/watch?v=TDAXvOoNWQI&t=77s     
```

### 2. Ubuntu Installation and assign partition
```bash
Ubuntu: (main) https://youngil.tistory.com/100
        (reference) https://dora-guide.com/ubuntu-download/
        
Alienware setting
1. Booting Bios Setup: https://www.youtube.com/watch?v=0nA4xU1Nr3g
```        

### 3. Ubuntu Korean Setting
```bash
https://www.youtube.com/watch?v=vqYfJow24L0
```

### 4. Install Anaconda
```bash
1. Go to Anaconda Web and press Download: https://www.anaconda.com/
2. ~/Downloads$ sha256sum Anaconda3–2021.11–Linux–x86_64.sh
3. ~/Downloads$ bash Anaconda3-2021.11-Linux-x86_64.sh

```

### 5. ROS Noetic
```bash
Reference YouTube: https://www.youtube.com/watch?v=ZA7u2XPmnlo
Noetic Web: http://wiki.ros.org/noetic/Installation/Ubuntu

1. ~$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
2. ~$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
3. ~$ sudo apt update
4. ~$ sudo apt install ros-noetic-desktop-full

Environment Setting
1. echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
2. source ~/.bashrc
```

### 6. chicago_ws
```bash
~$ mkdir -p ~/catkin_ws/src

~$ cd ~/catkin_ws/src

~/catkin_wc/src$ catkin_init_workspace

~/catkin_wc/src$ cd ..

pip install -U rosdep rosinstall_generator wstool rosinstall six vcstools

~/catkin_ws$ catkin_make

# Error
# Unable to find either executable 'empy' or Python module 'em'...  try
# https://answers.ros.org/question/353111/following-installation-instructions-catkin_make-generates-a-cmake-error/
```

### 7. package folder inside of the workspace
```bash
reference: http://wiki.ros.org/ROS/Tutorials/CreatingPackage

~/chicago_ws/src$ catkin_create_pkg first_pkg std_msgs rospy roscpp cv_bridge pcl_conversions pcl_ros sensor_msgs visualization_msgs image_transport
```


### 6. Python - (1)Window (2)Ubuntu
```bash
1. Window: go to Python org and Download: https://www.python.org/
2. Ubuntu: https://www.youtube.com/watch?v=Br2xt6B57SA
```

### 7. Visual Studio Code - Window
```bash
1. go to VS Code and Download: https://code.visualstudio.com/
2. New file and save file on the folder that we want to save it.

# Install - Python
1. go to Extensions
2. search Python and install
3. search Code Runner
4. click the gear button and click the setting and go down until we find Code Actions On Save.
5. Press Edit in settings.json
6. add this line => "code-runner.runInTerminal": true

# Install and customize - Vim
1. go to Extensions
2. search Vim
3. Ctrl + Shift + P => settings => click Preferences: Open Settings (JSON)
```
### 8. CUDA
```bash
reference web to remove and install CUDA and cuDNN: https://wooriel.tistory.com/53

remove all of it: https://stackoverflow.com/questions/56431461/how-to-remove-cuda-completely-from-ubuntu

When nvidia-smi is not connected even though nvidia is setted on PC, change the security boot option to disable.
```
<img width="30" alt="IMG" src="https://user-images.githubusercontent.com/73331241/158287222-1899b183-d0d5-4abd-8f5c-fab63c9df186.png">

### 9. PyTorch
reference: https://varhowto.com/install-pytorch-ubuntu-20-04/
reference: https://wooriel.tistory.com/40

### 10. python pcl
reference: https://issueantenna.com/repo/lianghongzhuo/pointnetgpd/issues/47
```bash
SOLVED ubuntu 20.04

created conda environment with python=3.6 numpy=1.19.2 cython and activate the environment
sudo apt-get update
sudo apt-get install pcl-tools
sudo apt-get install libpcl-dev -y
conda config --add channels conda-forge
conda install -c sirokujira python-pcl
conda install -c jithinpr2 gtk3
conda install -y ipython

Then, go to your anaconda environment lib folder ( cd ~/anaconda3/envs/YOUR_ENV_NAME/lib)
and execute following 4 commands:
ln -s libboost_system.so.1.64.0 libboost_system.so.1.54.0
ln -s libboost_filesystem.so.1.64.0 libboost_filesystem.so.1.54.0
ln -s libboost_thread.so.1.64.0 libboost_thread.so.1.54.0
ln -s libboost_iostreams.so.1.64.0 libboost_iostreams.so.1.54.0
```

### Exception
#### 1. WSL 2
[T1. WSL 2 Installation.pdf](https://github.com/ChicagoPark/Ubuntu/files/8239224/T1.WSL.2.Installation.pdf)

#### 2. Google Calendar: https://blog.naver.com/hongganz/222499476158
