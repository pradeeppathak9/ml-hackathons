# Game of Deep Learning Hackathon - Computer Vision Hackathon

Link: https://datahack.analyticsvidhya.com/contest/game-of-deep-learning/

Private Leaderboard Rank: 11   
Private Leaderboard Score: 0.9794331759    
Public Leaderboard Rank: 13   
Public Leaderboard Score: 0.9840785318  

VM Specs while working out these steps
 - Google Colab with GPU
 
Environment:
 - Google Colab with Python3 
 
Libraries: 
 - fastai==1.0.52
 - numpy==1.16.4
 - pandas==0.24.2
 - sklearn==0.0
 
Execution Steps:
 - Download the Snapshot models and save them in a directory
 - Open godl_final_sub.ipynb 
 - Update the following path in the Notebook accordingly
         DATA_DIR: test and train csv location
         IMAGE_DIR = path to image folder
         SNAPSHOT_DIR = where pretrained models are saved
         OUTPUT_DIR = location to save the intermediary predictions and final predictions 
 - Run all the cells 
 - Final submission file "final_sub_with_random_tta.csv" will be saved in output directory.
 
godl_snapshot_training_fastai_densenet201_tta.ipynb is the notebook for training model. Not needed to generate submissions. 
