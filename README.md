# Gesture-Recognition
As a data scientist at a home electronics company which manufactures state of the art smart televisions, we want to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote. We use Recurrent Neural Network to train a model to understand the hand gestures which can be used to control the TV without using a remote.

## Table of Contents
* [General Info](#general-information)
* [Approach Followed](#approach-followed)
* [Conclusion](#conclusion)
* [Contact](#contact)

## General Information
The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

- Thumbs up:  Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: 'Jump' backwards 10 seconds
- Right swipe: 'Jump' forward 10 seconds  
- Stop: Pause the movie
 
The training data consists of a few hundred videos categorised into one of the five classes. 
Each video is a sequence of 30 frames (or images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.

## Approach Followed

### Architecture
Two types of architecture are tried for analyzing videos:
- Convolutions + RNN
- 3D Convolutional Network

### Generators
We gave built our own batch data generator that can take a batch of videos as input without any error. Image cropping, resizing and normalization are performed successfully.

## Conclusions
- A convolution 3D model is used to train the dataset.
- The follwoing experiments have been perofrmed to get the right model:
  - Decrease the batch size
  - Decrease the number of images/frames captured within the video
  - Decrease the image/frame size
  - Decrease the number of epochs
  - Simply the architecture by reducing the number of layers used in RNN
    
## Contact
Created by [@jenifer2409] - feel free to contact me!
