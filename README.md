# Classification-Paper-Gunting-Stone-with-VGG19
1. Business Understanding
In this stage, the business objective of the project is to classify hand drawings depicting scissors, stones, or paper. This can be used in simple game applications or hand gesture recognition for device control. The dataset has been prepared by dividing the images into train and validation folders, with proportions of 60% and 40%, respectively. In total, there are 1314 images for training and 874 images for validation.

2. Data Collecting
This code is used to download the dataset required for the project from the GitHub repository. This dataset contains the hand images used for classification.

3. Data Understanding:
This process involves extracting the dataset from the previously downloaded zip file. The dataset consists of hand images representing scissors, stone, and paper. These images were then divided into train and validation folders for training and model evaluation purposes.

4. Data Preprocessing:
At this stage, the loaded images were processed using data augmentation to increase the variety of the training dataset. This augmentation includes rotation, horizontal and vertical shifting, cropping, and flipping. This helps the model to learn from a wide variety of images.

5. Modeling:
The model architecture used was VGG19, which was pre-trained on the ImageNet dataset. Transfer learning is done by utilizing the weights already trained on VGG19 and replacing the last layer to suit the hand classification task. The model is followed by multiple Dense layers for further learning.

6. Evaluation:
The model was evaluated using a validation dataset to estimate the performance of the model. The metric used is accuracy. In addition, graphical visualization of accuracy and loss from training and validation is also presented to understand the trend of model performance.

7. Test:
Finally, the user can upload a hand image that the model wants to classify. The model will process the image and provide the corresponding class prediction (scissors, rock, or paper). This allows users to test the model directly with new images.
