# Product-Photography-using-Generative-AI

##Deep Learning Model:

Utilizes the DeepLabV3 model with a ResNet50 backbone, pre-trained using PyTorch, for semantic segmentation.
Takes an input image and predicts a binary mask distinguishing the foreground from the background.

##Foreground Extraction:

Defines a function (make_transparent_foreground) to create a transparent foreground based on the binary mask obtained from the model's predictions.

##Background Removal:

Defines a function (remove_background) that takes an input image, processes it through the deep learning model, and removes the background, returning the transparent foreground and a binary mask.

##Custom Background Integration:

Provides a function (custom_background) to combine the transparent foreground with a custom background.
Positions the foreground in the center of the custom background and pastes it, resulting in a final image.

