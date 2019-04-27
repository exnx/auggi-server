This package contains a Flask server to take an image file path and return a bristol scale prediction


# To run
1. run auggi_server.py - decides when to run an inference with an image.  Creates an Inference object and passes an image.



About each script:

full_inference.py - contains the main Inference class that creates all the necessary module objects to classify an image.
segmentor.py - produces a binary mask from an image
bbox_from_mask.py - produces bounding box coordinates from a binary mask
classifier_bristol.py - produces a bristol scale prediction from an image path and bounding box coordinates


Dependancies:

Python 3.6
Pytorch

imutils==0.5.1
Flask==1.0.2
numpy==1.14.5
opencv-python==3.4.2.17
Pillow==5.2.0
torchvision==0.2.1