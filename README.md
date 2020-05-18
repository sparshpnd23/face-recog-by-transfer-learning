# face-recog-by-transfer-learning

In this project, I have created a Face-Recognition model using the concept of **Feature Tuning**.

_**Step 1:**_ We start of by collecting our dataset. For this, I have used _Haarcascade FrontalFace._ I have collected 200 images of mine & my friend for training the model & 100 images each for testing the model.
You can use the following code to collect the images and prepare the dataset.

![](/fr/1.png)
![](/fr/2.png)

I have used the same block of code multiple times to collect all the training & testing images of me & my friend. You can collect images of more people as per your requirement.




_**Step 2:**_ Now, we import pre-created MobileNet model from keras.applications. We freeze the already trained layers by   _layer.trainable= False._


![](/fr/3.png)





_**Step 3:**_ We add layers as per our requirement. Here, I have used _Softmax_ activation function.

![](/fr/4.png)



_**Step 4:**_ Next, we load our dataset. We have used the augmentation technique to increase our dataset since the size of original dataset is too small for a good accuracy.

![](/fr/5.png)

We see that our dataset is successfully loaded.

![](/fr/6.png)


_**Step 5:**_ Now, we begin training our model.

![](/fr/7.png)
![](/fr/8.png)


We see that the epochs begin.
![](/fr/9.png)


The model has been effectively trained and ready to use. You can use this model for prediction.









