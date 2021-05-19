# Automatic Image Captioning System using Deep Learning
### System Overview
Automatic image captioning, in other words, generating natural language descriptions according to the content observed in an image, is an important part of scene understanding, which combines the knowledge of computer vision and natural language processing. The application of image caption is extensive and significant, for example, the realization of human-computer interaction. In this project, an automatic image caption generation system has been developed with a user-friendly UI that provides a caption to the user upon the upload of an image with proper extension.

### Deep Learning Model
- #### Image Feature Extractor:

Here we have used a pretrained VGG16 model to extract features from the images of flicker8k dataset. The pretarined weights can be downloaded from [here](https://github.com/fchollet/deep-learning-models/releases/download/v0.1/vgg16_weights_tf_dim_ordering_tf_kernels.h5).

- #### Sequence Processor:

A  Long Short-Term Memory (LSTM) based model has been developed for training the text dataset of flicker8k. 

- #### Decoder:

Both the feature extractor and sequence processor output a fixed-length vector. These are merged together and processed by a Dense layer to make a final prediction.

### User Interface:
Flask has been used to develop the UI through which user can get captions for new images. It has certain features:
- Upload image option
- Checking allowed extensions of image
- Generate caption option that when clicked, acquires captions of image from the saved model and display it to the users
- Displaying uploaded image

#### *Before Uploading Image::*
![Alt text](images/gui1.png?raw=true "Title")
#### *After Uploading Image:*
![Alt text](images/gui3.png?raw=true "Title")
#### *Checking Allowed Extensions of Image (Error Message):*
![Alt text](images/gui5.png?raw=true "Title")
#### *After clicking Generate Caption option:*
![Alt text](images/gui4.png?raw=true "Title")
#### *After clicking Generate Caption option Without Uploading Image:*
![Alt text](images/gui2.png?raw=true "Title")
