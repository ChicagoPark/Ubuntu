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

### 6. Python - Window
```bash
1. go to Python org and Download: https://www.python.org/
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



### Exception
#### 1. WSL 2
[T1. WSL 2 Installation.pdf](https://github.com/ChicagoPark/Ubuntu/files/8239224/T1.WSL.2.Installation.pdf)

