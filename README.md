# Object Detector with Vision and Core ML

## Overview
The app in this sample identifies the most prominent object in an image by using MobileNet,
an open source image classifier model that recognizes around 1,000 different categories.

## Screenshot

Initial Screen             |  Camera Screen
:-------------------------:|:-------------------------:
![Initial Screen](https://user-images.githubusercontent.com/62091371/205447846-6a2877d4-1ef4-460f-b109-2a62136d0940.png)  |  ![Camera Screen](https://user-images.githubusercontent.com/62091371/205447833-4466870e-9b67-4e94-9100-9f1e85fa3765.png)


## How to use
Each time a user selects a photo from the library or takes a photo with a camera,
the app passes it to a [Vision][Vision] image classification request.
Vision resizes and crops the photo to meet the MobileNet model's constraints for its image input,
and then passes the photo to the model using the [Core ML][Core ML] framework behind the scenes.
Once the model generates a prediction, Vision relays it back to the app, which presents the results to the user.

## How it works
Crop and scale photos using the Vision framework and classify them with a Core ML model.
