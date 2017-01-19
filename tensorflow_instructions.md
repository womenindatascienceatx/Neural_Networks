## Linux/Mac OS X, Python 2.7/3.4/3.5:

### 1. Create a conda environment called tensorflow:

####  Python 2.7
`$ conda create -n tensorflow python=2.7`

#### Python 3.4
`$ conda create -n tensorflow python=3.4`

#### Python 3.5
`$ conda create -n tensorflow python=3.5`

### 2. Acitvate conda environment

`$ souce activate tensorflow`

`(tensorflow)$  # Your prompt should change`


## 3. Install Tensorflow using PIP

It is very important to use PIP and not conda to install.  The current version of tensorflow is buggy but we can install the old version with PIP.


### 3.1 Pick your binary  
#### Mac OS X, CPU only   
##### Python 2.7:

`(tensorflow)$ export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-0.10.0-py2-none-any.whl`

##### Python 3.4 or 3.5:
`(tensorflow)$ export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/mac/cpu/tensorflow-0.10.0-py3-none-any.whl`

#### Ubuntu/Linux 64-bit, CPU only
##### Python 2.7
`(tensorflow)$ export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.10.0-cp27-none-linux_x86_64.whl`

##### Python 3.5
`(tensorflow)$ export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.10.0-cp35-cp35m-linux_x86_64.whl`


### 3.2 FINALLY install tensorflow OS X and Ubuntu/Linux!

#### Python 2
`(tensorflow)$ pip install --upgrade $TF_BINARY_URL`

#### Python 3
`(tensorflow)$ pip3 install --upgrade $TF_BINARY_URL`



## Windows

TensorFlow requires MSVCP140.DLL, which may not be installed on your system. If, when you import tensorflow as tf, you see an error about No module named "\_pywrap_tensorflow" and/or DLL load failed, check whether MSVCP140.DLL is in your %PATH% and, if not, you should install the Visual C++ 2015 redistributable (x64 version).

Make sure you have Anaconda installed and up to date.

Tensorflow only works with python 3.5 in Windows.

#### Using cmd as your shell enter the following commands

##### 1. Create environment
`conda create -n tensorflow python=3.5`

##### 2. Activate environment
`activate tensorflow`

##### 3. Use pip to install tensorflow

 `pip install --upgrade https://storage.googleapis.com/tensorflow/windows/cpu/tensorflow-0.12.1-cp35-cp35m-win_amd64.whl`

## Install packages for workshop
##### Basic packages for visualization and running code:   
 `pip install jupyter`  
 `conda install matplotlib`   
 `conda install pandas`  
##### Neural network package:  
 `pip install keras`  
##### Image processing:  
 `pip install h5py`  
 `pip install pillow`
