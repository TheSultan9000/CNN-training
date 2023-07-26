# Deep neural network training

...
## Example of training a deep neural network

...
### Description:
This notebook demonstrates the training of a CNN to classify images into three categories (softmax)-
* Animals
* Building
* Nature

The model was largly trained on images of the English countryside and has a Precision: 1, Recall: 0.9, Accuracy: 0.6.

The resulting CNN can be seen in use within the following project:
- <a href="https://github.com/TheSultan9000/CNN-and-LLM-Flask-application">https://github.com/TheSultan9000/CNN-and-LLM-Flask-application</a>

...
### Installation and use:
- This project was made with the intention to learn how deep neural networks are trained. Therefore it is advised to understand how each component works and utalise these techniques in parallel projects.

Directory:
* Root folder
    * CNN_building.ipynb - a notebook file which outlines the logic behind the steps to traine a CNN
* CNN images- an lfs upload contianing example images to train the CNN
* logs- an empty directory to store logs whilst raining and testing the CNN

...
### Dependencies
Created using python version Python 3.10.9
```python
import tensorflow as tf
import os
import cv2
import imghdr
import numpy as np
from matplotlib import pyplot as plt
from keras.models import Sequential
from keras.layers import Conv2D, MaxPooling2D, Dense, Flatten, Dropout
from keras.metrics import Precision, Recall, BinaryAccuracy
```

...
### Contributions
Although contributions and comments are always welcome, please be aware that is project was used as a learning excersise and is not being activally maintained.