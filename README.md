# Cat Breed Prediction from Images

This project aims to predict cat breeds from images using convolutional neural networks.

## Dataset

The dataset used is from Kaggle: https://www.kaggle.com/datasets/zippyz/cats-faces

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

Dataset source: https://www.kaggle.com/datasets/zippyz/cats-faces

Research paper for EfficientNet architecture: https://arxiv.org/abs/1905.11946
