1 - Update and Install the basic tools

sudo apt-get update

sudo apt-get upgrade 

sudo apt-get install htop vim tmux 

2 - Setup pip without sudo

Download https://bootstrap.pypa.io/get-pip.py

Run python get-pip.py --user

It will install it into \~/.local/

Add PATH=$PATH:~/.local/bin to bashrc or bash_profile

3 - Setup python tools

pip install virtualenv numpy scipy ipython pdbpp tqdm scikit-learn scikit-image six wheel pandas matplotlib pdbpp sympy nose

4 - Install Nvidia Drivers

Add graphics-drivers ppa and install the official release: https://launchpad.net/~graphics-drivers/+archive/ubuntu/ppa

5 - Download CUDA toolkit and set it up

https://developer.nvidia.com/cuda-toolkit and download the toolkit. If you need an earlier release go to legacy releases and the end of the page

Add cuda/bin to $PATH and cuda/lib64 to $LD_LIBRARY_PATH

!!WHEN IT ASKS YOU TO INSTALL THE NVIDIA DRIVERS SAY NO, WE ALREADY SET THAT UP. It might break things

6 - Download CUDNN and copy it inside the cuda folder. DONT DOWNLOAD THE DEB RELEASE

7 - Install ffmpeg

8 - Install opencv

Dependencies:

sudo apt install gcc g++ git libjpeg-dev libpng-dev libtiff5-dev libjasper-dev libavcodec-dev libavformat-dev libswscale-dev pkg-config cmake libgtk2.0-dev libeigen3-dev libtheora-dev libvorbis-dev libxvidcore-dev libx264-dev sphinx-common libtbb-dev yasm libfaac-dev libopencore-amrnb-dev libopencore-amrwb-dev libopenexr-dev libgstreamer-plugins-base1.0-dev libavcodec-dev libavutil-dev libavfilter-dev libavformat-dev libavresample-dev

Install VLC for codecs and stuff

wget https://github.com/opencv/opencv/archive/3.3.0.zip
wget https://github.com/opencv/opencv_contrib/archive/3.3.0.zip

