# Automatic Image Captioning System using Deep Learning
Automatic image captioning, in other words, generating natural language descriptions according to the content observed in an image, is an important part of scene understanding, which combines the knowledge of computer vision and natural language processing. The application of image caption is extensive and significant, for example, the realization of human-computer interaction. In this project, an automatic image caption generation system has been developed with a user-friendly UI that provides a caption to the user upon the upload of an image with proper extension.

Here we have used a pretrained VGG16 model to extract features
from a given image and retrained the model with flicker8k dataset of images. 
Later, this dataset is used for training the final deep learning model. Finally, Flask has been used to develop the UI through which user can get captions for new images.
