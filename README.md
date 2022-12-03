# Object Detector with Vision and Core ML

## Overview
The app in this sample identifies the most prominent object in an image by using MobileNet,
an open source image classifier model that recognizes around 1,000 different categories.

## How to use
Each time a user selects a photo from the library or takes a photo with a camera,
the app passes it to a [Vision][Vision] image classification request.
Vision resizes and crops the photo to meet the MobileNet model's constraints for its image input,
and then passes the photo to the model using the [Core ML][Core ML] framework behind the scenes.
Once the model generates a prediction, Vision relays it back to the app, which presents the results to the user.

## How it works
Crop and scale photos using the Vision framework and classify them with a Core ML model.
