# Deep Space Radio Signal Classification with CNN using SETI Spectrograms.
In this project, the primary goal is to classify deep space radio signals into one of four categories using a Convolutional Neural Network (CNN) built with Keras and TensorFlow. The dataset comprises 2D spectrograms collected by the Allen Telescope Array at the SETI Institute. These spectrograms are treated as images for the purpose of training the CNN.

## The workflow consists of several key steps:
Data Preprocessing: Initially, the project begins by displaying the 2D spectrograms using Matplotlib for visualization. The input data is reshaped using NumPy to meet the requirements of the CNN.

Data Augmentation: Data augmentation is applied using the ImageDataGenerator, a powerful tool for generating augmented training data. This helps improve the model's generalization by exposing it to various transformations of the original data.

CNN Model Creation: A Convolutional Neural Network (CNN) is designed, consisting of two convolutional layers and one fully connected layer. The model uses the Adam optimizer, categorical crossentropy as the loss function, and accuracy as the evaluation metric.

Learning Rate Scheduling: During training, a learning rate scheduling technique is applied. It progressively reduces the learning rate as training advances, which can enhance the model's convergence.

Model Training: The CNN is trained using the fit() method. ModelCheckpoint() is utilized to save the model weights associated with the highest validation accuracy after each epoch. This is useful for later transfer learning or fine-tuning.

Model Evaluation: The trained CNN is evaluated to assess its performance. This involves using the model to make predictions and measuring metrics like accuracy.

While this project focuses on building a basic image classifier for SETI data, it introduces valuable concepts such as data augmentation, learning rate scheduling, and weight-saving techniques. These skills can be further extended and applied to more advanced projects in image classification and deep learning.
 
  
