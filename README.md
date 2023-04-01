# EMINIST_Lettter_dataset_val-acc-99.4-

In several research articles, Digits-recognition detection is done through the application of Machine Learning and Deep Learning algorithms. 
When these systems are applied to https://www.itl.nist.gov/iaui/vip/cs_links/EMNIST/matlab.zip , recognition is done very quickly and greater accuracy.

# Dataset link :
https://www.kaggle.com/datasets/crawford/emnist

# Instructions
1) Save the model in .hdf5 format
2) run the program with certain test data


# Introduction:

In this project 
we implemented a system for recognizing handwritten digits using a Convolutional
Neural Network (CNN). The system is trained on the EMNIST Digits dataset, which consists of images of
digits across 10 distinct classes.
Dataset and Preprocessing
The EMNIST Digits dataset is an extension of the original MNIST dataset, containing only digits, with a
total of 280,000 images. We loaded the dataset and split it into training and testing sets. Then, we
normalized the pixel values by dividing them by 255 to obtain a range of 0 to 1. We also one-hot encoded
the labels to prepare them for use with the CNN.
CNN Model Architecture and Training
We designed a CNN architecture that includes convolutional layers, pooling layers, dropout layers for
regularization, and fully connected layers. The model is compiled with the categorical_crossentropy loss
function, the Adam optimizer, and the accuracy metric. We used early stopping to prevent overfitting
and monitored the training time.
Model Evaluation
After training, we evaluated the model's performance on the testing set. We plotted the training and
validation accuracy and loss values to visualize the model's performance throughout training.
Prediction
We tested the model on new instances from the test set, displaying the images and making predictions
using the saved model. The model correctly predicted the digit classes for the selected images.
Conclusion
This project demonstrates the effectiveness of CNNs for handwritten digit recognition. By training a CNN
on the EMNIST Digits dataset, we achieved an accuracy of approximately 99.4% on the test set, enabling
accurate recognition of digits from new instances.
Project Code Overview
1. Download and extract the EMNIST dataset
2. Load the dataset and split it into training and testing sets
3. Normalize the pixel values and one-hot encode the labels
4. Define the CNN architecture and compile the model
5. Train the model with early stopping
6. Evaluate the model's performance on the testing set
7. Save the trained model
8. Test the model on new instances from the test set and display the images
9. Make predictions using the saved model and print the results

# Steps to be followed :
By following these steps, we built a functional system for recognizing handwritten digits using a
Convolutional Neural Network and the EMNIST Digits dataset.
Adapting the Model to Different EMNIST Datasets
The EMNIST dataset is an extension of the original MNIST dataset and consists of six subsets: ByClass,
ByMerge, Balanced, Letters, Digits, and MNIST. Each subset has a different number of classes, ranging
from 10 (Digits) to 62 (ByClass). To adapt the model for different subsets, the only change needed in the
CNN architecture is to adjust the number of units in the final dense layer to match the number of classes
in the chosen dataset. For example, if you want to use the EMNIST ByClass dataset with 62 classes, you
would need to change the final dense layer to have 62 units, like this: model.add(Dense(62,
activation="softmax"))
Keep exploring, experimenting, and refining your skills. Happy learning!
References Cohen, G., Afshar, S., Tapson, J., & van Schaik, A. (2017). EMNIST: an extension of MNIST to
handwritten letters. Retrieved from https://arxiv.org/abs/1702.05373 .
