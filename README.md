# Covolutional-Dog-Breed-App
A dog breed classifier which uses convolutional neural networks.

# About and Procedure
- Uses convoluitonal neural network to predict the breed of a dog, if the input images is a dog image. Else, If image is human, returns a resembling breed of dog.
- Here, we trained 2 models with different apporach - one from scatch and other using transfer learning.
- We analyze both the models and determine the complexity of creating a model from scratch by understanding the advantages of transfer learning.
- This project uses the convolutional layers to extract complex features from images in oreder to classify from the feature map created for every input image. To learn more about   CNN, refer to this [link](https://www.analyticsvidhya.com/blog/2021/05/convolutional-neural-networks-cnn/). 
- The general approach followed was-
  - First import the datasets to btrained upon.
  - Create method to detect human face.
  - Create the model architecture from scratch and transfer learning separately and train in them separately.
  - Tune hyperparameter based on how the validation accuracy shows a lower trend and setlle on parameters that provide a acceptable validation loss.
  - We save the best model based on the lowest validation loss provided by the model.
  - After tarining, test on both the models to analyse the perofmance.

# Results obtained
- Ater tuning the hyperaparameters for hours, I was able to achieven an accuracy of about <b>14%</b> on my test datasets, if the model created was from scratch. The accuracy could have been improved if used some advanced techniques while creating the model architecture or using momentum, providing learning rate decay etc.
- Whereas, I achieved an accuracy of about <b>86%</b> if I use transfer learning concept to create my model architecture thus proving the usefullness of transfer learning.

<b>Results for random input images</b>

=> Image-1

=> You are a human!

![image](https://user-images.githubusercontent.com/36024003/127344793-883d320d-5f64-4391-ac2c-9553819b00f6.png)

- Predicted index- 47
- Hey Human! You look like a Chihuahua!


=> Image-3

=> Hi Dog! How are you?

![image](https://user-images.githubusercontent.com/36024003/127345068-c04cc113-cb31-4aee-8400-5e7d946c212f.png)

- Predicted index- 22
- Your family is Bernese mountain dog!



=> Image-7

=> Hi Dog! How are you?

![image](https://user-images.githubusercontent.com/36024003/127345418-c38fc734-4bd8-401d-9ccb-da64b1316a21.png)

- Predicted index- 1
- Your family is Afghan hound!
