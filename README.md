# RL-video-summarization

This repo contains the Pytorch implementation of the AAAI'18 paper - [Deep Reinforcement Learning for Unsupervised Video Summarization with Diversity-Representativeness Reward](https://arxiv.org/abs/1801.00054). 

# Requirenments
The main requirements are Pytorch 1.9.1 and python 3.9.  Please install other missing dependencies that are presented in the requirements.txt.

# Using
## Raw datasets
First of all, you need to download raw datasets (mp4 files) from HERE and unzip them to the datasets folder in the root folder of the project. 

After that you should open the file notebooks/Pipeline.ipynb to generate the dataset, train, and inference.

## Generate dataset from videos

In the notebooks/Pipeline.ipynb notebook you should run the corresponding cells. If you are running it for the individual video video_path should contain the path to it, if there is more than 1 video - video_path should contain the path to the directory. In both cases, the prepared dataset will be stored in the file datasets/{output_dataset_name} with h5 extension.

## Generate dataset from videos



