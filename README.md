# CV DL | Сlothing classification by image

<p align="center">
  <img src="image_to_report\clo.jpg" width="600">
</p>

I'm implementing clothing image classification using deep learning. For this, I'll be using TensorFlow and Keras.

You can find clothing datasets for training and testing the model at the following link - https://github.com/alexeygrigorev/clothing-dataset-small.git

Remark: comments in the code will be written in Russian

## Training, quality assessment
[main](main.ipynb) - The main program code is presented in this notebook. I used a pretrained model in ImageNet (Xception) and adapted it to my data. To do this, I retained all the convolutional layers and recreated the dense layers. I also used dropout to regularize the model and preprocessed the images (to increase their number).

## Result
The trained model was tested on a dedicated test data set and showed 81% accuracy. The reason may be the size of the images I used, I used 150x150, the quality can be significantly improved if you use 299х299, another possible reason is an insufficient number of training images
