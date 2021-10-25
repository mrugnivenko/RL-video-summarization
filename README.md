# RL-video-summarization

This repo contains the Pytorch implementation of the AAAI'18 paper - [Deep Reinforcement Learning for Unsupervised Video Summarization with Diversity-Representativeness Reward](https://arxiv.org/abs/1801.00054). 

# Requirenments
The main requirements are Pytorch 1.9.1 and python 3.9.  Please install other missing dependencies that are presented in the requirements.txt.

# Using
## Raw datasets
First of all you need to download raw datasets (mp4 files) from HERE and uzip it to the datasets folder in the root folder of the project. 

After that you should open the file notebooks/Pipeline.ipynb to generate dataset, train and inference.

## Generate dataset from videos

In the notebooks/Pipeline.ipynb notebook you should run the corresponding cells. If you are running it for the individul video video_path should contain the path to it, if there are more then 1 video - video_path should contain path to the dirrectory. In both cases prepared dataset will be stored in the file datasets/{output_dataset_name} with h5 extention.

## Generate dataset from videos



