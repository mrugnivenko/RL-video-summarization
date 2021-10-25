# RL-video-summarization

This repo contains the Pytorch implementation of the AAAI'18 paper - [Deep Reinforcement Learning for Unsupervised Video Summarization with Diversity-Representativeness Reward](https://arxiv.org/abs/1801.00054). 

# Requirenments
The main requirements are Pytorch 1.9.1 and python 3.9.  Please install other missing dependencies that are presented in the requirements.txt.

# Using
## Raw datasets
First of all you need to download raw datasets (mp4 files) from https://drive.google.com/file/d/1wCOzakc5ikOJWTPLoTvZetHFXpJABdww/view and uzip it to the datasets folder in the root folder of the project. 

After that you should open the file notebooks/Pipeline.ipynb to generate dataset, train and inference.

## Generate dataset from videos

In the notebooks/Pipeline.ipynb notebook you should run the corresponding cells. If you are running it for the individul video video_path should contain the path to it, if there are more then 1 video - video_path should contain path to the dirrectory. In both cases prepared dataset will be stored in the file datasets/{output_dataset_name} with h5 extention.

## Split dataset

In the same notebook you should run "Split dataset on train and test" cell to split dataset into train and test.

## Train and test model

To train model you should run the cells. By default DR-DSN method is used. To train sup-DSN you should add "--is-sup 1". To train D-DSN add "--d-dsn 1" and to train R-DSN - "--r-dsn 1".

Testing can be done with "Test model with RL" cells and the same set of the arguments for different methods. 

## Get video summary

The final thing that can be done with notebooks/Pipeline.ipynb notebook is video summary. It should be done after model testing stage. -p flag corresponds to the log file with h5 extention returned by the test. --save-name is the output name.





