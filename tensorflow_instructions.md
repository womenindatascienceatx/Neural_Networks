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


### 3. Install Tensorflow using conda

A community maintained conda package is available from conda-forge.

Only the CPU version of TensorFlow is available at the moment and can be installed in the conda environment for Python 2 or Python 3.

`(tensorflow)$ conda install -c conda-forge tensorflow`

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
