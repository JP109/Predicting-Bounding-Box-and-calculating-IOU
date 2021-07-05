# Predicting-Bounding-Box-and-calculating-IOU
This notebook was created to practice creating bounding boxes on images, and validating them using IoU calculations.

We will be creating bounding boxes on bird images from Caltech Bird Dataset. The dataset was stored in google drive, which was mounted onto the colab.

We used Transfer Learning on MobileNetv2 with pretrained imageNet weights for the feature extractor part of the model, and used simple Pooling and Dense layers for the Classifier part, which was fed the output of the Feature Extractor part as input, using Tensoflows functional API. As outputting a bounding box is a regression task(The coordinates of the bounding box are predicted), we used a Dense layer, which was fed the output of the Classifier part.


