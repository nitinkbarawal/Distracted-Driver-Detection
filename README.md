# Distracted-Driver-Detection using CNN with Transfer Learning (Using Fine-tuned VGG19
Model)

I have created a instance of ImageDataGenerator which does all preprocessing operations on images that we are going to feed to our CNN.

Loading only 32 images at once into memory and performing all the preprocessing operations on loaded images.The flow_from_directory loads a defined set of images from the location of images, instead of loading all images at once into memory.
  
  train_generator contains training set
  
  val_generator contains validation set
  

Going to load a VGG19 model, without top Fully connected layers, with its trained weights(imagenet) Then we are going add Fully Connected Layers on top of MaxPooling2D layer.

Leaving the last 2-3 layers, the weights of all other layers of VGG19 have been freezed


