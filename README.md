# Udacity_Dog_Project
Final "capstone" project - Udacity data science nanodegree

# Project Overview
This project is part of the Udacity data science nanodegree program. The objective is to train and use a CNN to create a web application which can distinguish between dog breeds. 

# Problem Statement
The objective is to 1) differentiate between dogs and humans and 2) identify the dog breed (and the dog breed a human mostly resembles). This has to be accessable via a web application, which can be hosted locally. 

# Metrics
- Model accuracy has to be quanitifed, as is done in the notebook. 
- The resulting model(s) are accessable via a locally hosted web application, which can identify dog breeds.
- The code is stored in a github repository.

# Disclaimer 
This project uses pre-trained models from amazom (`VGG16Data` and `Resnet50`) and is based on a template by Udacity (`git clone https://github.com/udacity/dog-project.git`). 

# Setting up environment and downloading training data

The best way to 
1. Clone the repository and navigate to the downloaded folder.

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place its contents in the repo, at location `./dogImages` (where `.` is your project workspace, probably "dog-project"). 

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place its contents in the repo, at location `./lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

4. Download the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `./bottleneck_features`.

5. Download the [Resnet50 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogResnet50Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.

6. Create a fresh conda environment and install the required packages. Linux: `conda env create -f requirements/dog-linux.yml`; Windows: `conda env create -f requirements/dog-windows.yml`; Mac: `conda env create -f requirements/dog-mac.yml`.

7. Activate your environment `conda activate dog-project`.

# Running the breed identifier
A prerequisite for this project is to evaluate the CNN, Which was done in a jupyter notebook. For simplicity, the web app is run directly from the jupyter notebook. In order to train a CNN and run the web app, run the jupyter notebook `dog_app.ipynb` (install jupyter if required). The last cell of the notebook will have a link to the web app.
