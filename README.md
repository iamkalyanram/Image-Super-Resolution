# Image-Super-Resolution
SRGAN(super Resolution Generative Adversarial Network) is a generative adversarial network for single image super-resolution. It uses a perceptual loss function which consists of an adversarial loss and a content loss. The adversarial loss pushes the solution to the natural image manifold using a discriminator network that is trained to differentiate between the super-resolved images and original photo-realistic images. In addition, the authors use a content loss motivated by perceptual similarity instead of similarity in pixel space.

# Dataset:
Flickr2k images\
https://drive.google.com/drive/folders/1B-uaxvV9qeuQ-t7MFiN1oEdA6dKnj2vW \

# Packages for Installation:
Tensorflow, Opencv-Python , Sklearn

# Steps that to be followed
Note: In this model we try to use the input image of shape (32,32) and output image as (128,128) due to avoid the high computation (usually GAN taken more time to train)\
Step1: Download the folder “fickr2k” containing images from the above google drive link.\
Step2: Reshape the each image from the downloaded folder(fickr2k) to (32,32) and save it in Lr folder which act as input to the SRGAN.\
Step3: Reshape the each image from the downloaded folder(fickr2k) to (128,128) and save it in Hr folder ,which act as output your model.\
\
Note: Here we reshape the downloaded images twice one to (32,32) and save it in LR folder and second one to (128,128) and save it in Hr folder and the both folders should have the same name of the image one of (32,32) and other having (128,128) size.\
\
Step4: Now give the correct path Lr,Hr folder in the code in the main.py file ,each epoch takes 15-20 minutes so we used 20 epochs (If you have high computation power you can increase the no.of epochs) and execute the main.py file.\
\
\
After all epochs are completed you can see your output, if you are not satisfied with the
resolution train the model again.
