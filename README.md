# CMC MSU. Graphics course. Template for Ray Marching task

This is better template for task of Ray Marching for "Computer Graphics" course in CMC MSU 2019.

## Requirements

You need C++ compiler, CMake, make, OpenGL 3.3+ and GLFW3 library

To install everything, **except GLFW3** you can run this

`sudo apt install mesa-utils xorg-dev libglu1-mesa-dev cmake make build-essential`

To install GLFW3, you can download, unzip, compile it on your own computer and install (I think you can do it easier, but I have script only for this):
```
sudo apt install unzip cmake make && \
wget "https://github.com/glfw/glfw/releases/download/3.2.1/glfw-3.2.1.zip" && \
unzip glfw-3.2.1.zip && \
cd glfw-3.2.1 && \
sudo cmake -G "Unix Makefiles" && \
sudo make && \
sudo make install && \
cd .. && \
sudo rm -f glfw-3.2.1.zip && \
sudo rm -rf glfw-3.2.1
```

## Installation and Run

0. Clone the repository and go to folder where it was cloned.
`git clone https://github.com/CrafterKolyan/cmc-msu-graphics-template-raymarching.git && cd cmc-msu-graphics-template-raymarching`
1. Create build folder and go to it. `mkdir build && cd build`
2. `cmake ..`
3. `make`
4. `./main`

If any error occured, please read the "Requirements" section.

## Enhancements done to the standard template

1. No compilation error on MAC OS X
2. Shaders are now copied on build and also are thought to be source files
3. All files are reformated (4 space identation)
