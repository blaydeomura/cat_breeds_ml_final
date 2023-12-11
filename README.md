# Cat Breed Prediction from Images

This project aims to predict cat breeds from images using convolutional neural networks.

## Dataset

The dataset used is from Kaggle: https://www.kaggle.com/datasets/yapwh1208/cats-breed-dataset/data

It contains 953 images of cat faces from 5 popular breeds:
- Bengal 
- Ragdoll
- Siamese  
- Maine Coon
- Domestic Shorthair

The images are 180 x 180 (re-sized) color images in JPG format.

## Models

Several models were trained:

- **Baseline CNN** - Simple 3 layer convolutional neural network 
- **Regularized Model** - Added regularization techniques like dropout to reduce overfitting
- **Augmented Model** - Used augmented images to increase dataset size
- **EfficientNet** - Pre-trained EfficientNet model using transfer learning

## Results

The pre-trained EfficientNet model performed best by far, achieving ~88% validation accuracy. The augmented model performed worse likely due to overfitting on duplicated augmented images.

## Reference

Dataset source: 
https://www.kaggle.com/datasets/yapwh1208/cats-breed-dataset/data

Akvelon's MeowTalk, AI/ML based cat translator: 
https://medium.com/@dmitry.astankov/cat-breed-classification-with-deep-learning-169c66b3c478

Research paper for EfficientNet architecture: 
https://www.researchgate.net/publication/344410350_Classification_and_understanding_of_cloud_structures_via_satellite_images_with_EfficientUNet
