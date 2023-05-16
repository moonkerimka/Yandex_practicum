## Determining a person's age from a photo

### Tool stack

The keras library: using ResNet architectures.
Testing various methods of image augmentation.

### Input data

A large store is developing a machine vision system. The model will help to offer goods to different age groups and check the age of the buyer of alcohol.

There is marked data: photographs of people with age indication.

### Target

Build a model that will determine the approximate age of a person from a photograph. The MAE metric should not exceed 8 points.

### Project structure

1. Analyze available data: number of photos, size, age groups;
2. Prepare data: create datagens, scale and perform augmentation;
3. Create and train a neural network. Test different architectures. Calculate the quality of the model.

### General conclusion

The purpose of the study is fulfilled: the trained model demonstrates MAE = 6.27 without parameter tuning and data augmentation.

The initial data contained 7.5 thousand records, without gaps and outliers. Most of the people in the photographs are in the age range of 20-30 years. The final model contains the ResNet architecture and convolutional layers pre-trained on ImageNet.

#### *Important*

The model was trained on a separate training server.
The server did not skip new solutions if the required metric was reached. Successful training took place the first time and the training server did not allow new models to be run again.
The project contains a text record of the model and a training log.
