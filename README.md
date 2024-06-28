# Image-Classification-CNN



# Deep Learning Model Training and Evaluation

## Introduction
This repository contains code for training a deep learning model using TensorFlow/Keras. The model is trained on a dataset split into training, validation, and test sets. After training, the model's performance is evaluated on both validation and test data.

## Dataset Structure
Before running the training script, ensure your dataset is structured as follows:(THIS CONTAISN THE IMAGES WHICH ARE GIVEN AS INPUTS TO TRAIN AND TEST)

```
Dataset/
│
├── train/
│   ├── img1/
│   ├── img2/
│   └── ...
│
├── val/
│   ├── img1/
│   ├── img2/
│   └── ...
│
└── test/
    ├── img1/
    ├── img2/
    └── ...
```

- **train/**: Contains training images divided into subdirectories by class.
- **val/**: Contains validation images, similarly organized by class.
- **test/**: Contains test images, organized by class.

## Steps to Train and Evaluate the Model
1. **Training the Model**
   - Run `train.py` to start training the model. This script will save the trained model architecture (`model.json`) and weights (`model.weights.h5`) in the current directory.

   ```bash
   python train.py
   ```

2. **Validation**
   - After training, you can validate the trained model using the validation set.
 

3. **Testing**
   - Finally, test the trained model on unseen data using the test set.
   - Modify `test.py` to load the saved model and perform inference on the test set.

   ```bash
   python test.py
   ```

## Notes
- Make sure to install the required dependencies (`tensorflow`, `keras`, etc.) before running the scripts.
- Adjust hyperparameters, data augmentation settings, and other configurations as needed in `train.py`,  `test.py`.

