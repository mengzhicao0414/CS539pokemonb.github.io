# CS539pokemonb.github.io
## overview
This project contains two parts.Part 1 is about the prediction of battle result between two pokemons, while part 2 is the iamge generation using Generative Adversarial Networks<br>    
## Dependencies(pip install)
Numpy<br>
Pandas<br/>
Tensorflow<br/>
cv2<br/>
matplotlib<br/>
seaborn<br/>
prettytable<br/>
itertools<br/>
time<br/>
scikit-learn<br/>
SciPy<br/>
## Part1
### Introduction
First we conduct data visualization feature engineering and elo-rating , then we try several classical machine learning models to predict the combat result. The models include logistical regression, SVM, KNN, Adaboost, and MLP and so on. And we plot each model’s confusion matrix, and ROC curve. <br>
### File
The file contains data and code, the data part contains combats.csv and pokemon.csv.<br> 
The code has five parts: data visualization, feature engineering, elo-rating and algorithms<br/> 
## Part 2
### Introduction
Generative adversarial networks are a class of artificial intelligence algorithms used in unsupervised machine learning, implemented by a system of two neural networks contesting with each other in a zero-sum game framework.
### File
### Usage
#### Code_1
python resize.py<br/>
python rgb.py<br/>
python GAN.py<br/>
#### Code_2
you can use our dataset to train the model by

python main.py --input_height 64--input_width 64 --output_height 64 --output_width 64 --data pokemon --crop --train --epoch 80 --input_fname_pattern "*.jpg"

Or, you can use your own dataset, making sure data folder contains your dataset or you can use

$ mkdir data/DATA_NAME

then, add you images data into DATA_NAME folder and use our model by

python main.py --input_height **--input_width ** --output_height ** --output_width ** --data DATA_NAME --crop --train --epoch 80 --input_fname_pattern "*.jpg"


