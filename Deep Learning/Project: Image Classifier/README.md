# Udacity Machine Learning Basics Nanodegree

## Project 2: Create Your Own Image Classifier

Project code for Udacity's Machine Learning Basics Nanodegree program. In this project, I have build an image classifier using PyTorch, then converted it into command line applications: `train.py` and  `predict.py`.

Some of the features of this project are:
1. The Python code is an image classifier to recognize different species of flowers.
2. Dataset contains 102 flower categories.
3. Alexnet from torchvision.models pretrained models was used. It was loaded as a pre-trained network, based on which defined a new, untrained feed-forward network as a classifier, using ReLU activations and dropout.
4. Trained the classifier layers using backpropagation using the pre-trained network to get the features.
5. The loss and accuracy on the validation set were tracked to determine the best hyperparameters.
6. Command line applications `train.py` and `predict.py`
For command line applications there is an option to select either Alexnet or VGG13 models.

Following arguments are mandatory or optional for `train.py`

- `data_dir`. Provide data directory. Mandatory argument, type = str
- `--save_dir`. Provide saving directory. Optional argument, type = str
- `--arch`. Vgg13 can be used if this argument specified, otherwise Alexnet will be used, type = str
- `--learning_rate`. 'Learning rate, default value 0.001', type = float
- `--hidden_units`. Hidden units in Classifier. Default value is 512, type = int
- `--epochs`. Number of epochs, type = int
- `--gpu`. Option to use GPU, type = str

Following arguments are mandatory or optional for `predict.py`

- 'image_dir'. 'Provide path to image. Mandatory argument', type = str
- 'load_dir'. 'Provide path to checkpoint. Mandatory argument', type = str
- '--top_k'. 'Top K most likely classes. Optional', type = int
- '--category_names'. 'Mapping of categories to real names. JSON file name to be provided. Optional', type = str
- '--GPU'. "Option to use GPU. Optional", type = str
