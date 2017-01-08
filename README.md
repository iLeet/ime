Compiling
==========

First make sure that you have the necessary compiling, if any library is missing then you need to find it and install in your linux by yourself, required libraries are:

* wxWidgets >= 3.0
* Boost >= 1.55.0

### Windows
==============

Assuming that you have MSVC 2013 or later and the required libraries installed, clone the project, open the project file in `vcproj/Project/RME.vcproj` then hit build.

For more details you can follow [this tutorial](http://otland.net/threads/compiling-iLeets-map-editor-from-the-latest-source-with-msvc-2013.216826/) by dominique120.

### Linux
===============

```bash

# Installing dependencies
sudo apt-get install git cmake libboost-system-dev libboost-thread-dev libglu1-mesa-dev libwxgtk3.0-dev libarchive-dev freeglut3-dev libxmu-dev libxi-dev

# Clone the project
git clone https://github.com/hjnilsson/rme.git

# Go to RME Folder
cd rme

# Preparing to build
mkdir build && cd build
cmake ..

# Building
make -j `nproc`

# Running and enjoy
./rme
```

### macOS
===============
Install the package manager Homebrew: http://brew.sh
```bash

# Install dependencies
brew install git cmake wxmac boost libarchive

# Clone the project
git clone https://github.com/hjnilsson/rme.git

# Create a build directory and build
mkdir rme/build && cd rme/build && cmake .. && make

# Run
./rme

```
