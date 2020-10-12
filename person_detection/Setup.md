## Environment Setup Instruction for Assignment 2

We strongly advise you to use conda for managing the python and TensorFlow packages. Installing CUDA and other drivers can be quite daunting, and Conda takes care pretty much everything for you. To install conda, please follow the instruction [here](https://docs.anaconda.com/anaconda/install/windows/)

Once you have installed anaconda, please follow the instructions below:

1. Create a Conda environment

If you have a GPU:

``` $ conda create --name "cs249_gpu" python=3.7 tensorflow-gpu=1.15 Pillow contextlib2```

If you  don't have a GPU

``` $ conda create --name "cs249" python=3.7 tensorflow=1.15 Pillow contextlib2```


2. Once you have created a conda environment, activate and install the tf_slim package that is needed for this assignment

``` 
$ conda activate cs249 
```
```
(cs249)$ pip install --upgrade  tf_slim
```


3. Check if your TensorFlow install and tf_slim installation is correct

```
(cs249)$ python

```

```
>> import tensorflow as tf
>> tf.__version__
`1.15`
>> import tf_slim
```

If all the imports work without any errors, you are good to go.

If you are stuck with the setup, we have made a video that goes step-by-step. Check out the video [here](https://www.youtube.com/watch?v=6_BoM5_tFXk&feature=youtu.be)
