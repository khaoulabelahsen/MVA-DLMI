# MVA-DLMI
Deep Learning for Medical Imaging
Khaoula Belahsen - Nadir El Manouzi

# Data
The images from the training set and the test set are in the folders train and test.

The first cells are used to create paths to npy files which will be created in the next cell with the functions `create_train_data()` and `create_test_data()`.

`create_augmented_train_data()` can be used to create the augmented data set.

## Pre-trained models

Pre-trained models are available in the folder `res` 

without data augmentation : `unet_2heads.hdf5`, `r2unet.hdf5`, `unet_classic.hdf5`, `Nestnet.hdf5` and `AttResNet.hdf5`

with data augmentation : `unet_2heads_dataaug_rmsprop.hdf5` and `nestnet_aug.hdf5`

In the model choice part of the code, uncomment the model of your choice, put `data_augmentation = False` or `data_augmentation = True` depending on the dataset you want to use and uncomment the pre-trained path corresponding to the model chosen.

## Training

In the model choice part of the code, uncomment the model of your choice, put `data_augmentation = False` or `data_augmentation = True` depending of the dataset you want to use and uncomment `pretrained_path = None`

## Submission

For the U-Net with 2 heads, use `submission(two_outputs=True)`
For all the other models, use `submission(two_outputs=False)`

A file submission.csv will then be generated.

## Qualitative results
In order to have qualititative results on 3 different images, just run the last cell of the notebook.


