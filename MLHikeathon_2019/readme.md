# ML Hikeathon (An Online Machine Learning Hackathon)
  

Link: https://datahack.analyticsvidhya.com/contest/hikeathon/

Private Leaderboard Rank: 1  
Private Leaderboard Score: 0.9409118988  
Public Leaderboard Rank: 1  
Public Leaderboard Score: 0.9415281974  


VM Specs while working out these steps  
    Ram - 156 GB  
    CPU - 32 cores  
    Min free hard disk space - 100GB  
    
    
Environment Setup:  
    Install Anaconda Version - 4.5.2  
    Create Virtual Environment with Python- 2.7.15  
        and do pip install -r requirement.txt to install all the dependencies   


Execution Steps:  
Run the following notebooks in order (Files generated from one might be used in notebooks that follows later)  

1. undirected_graph_features.ipynb  
    Run time - around 30 hours   
    script generates following files, which is used in final model building  
        degrees_contact.pkl - degrees for the undirected contact graph  
        cluster_coeffs.pkl - cluster coefficients for the node pairs in the full data set  
        triangles.pkl - number of triangles for the node pairs in the full data set  
        jc_rsa_pa_aai.csv - graph features for the node pairs in the full data set  
       
2. directed_degrees_feature_creation.ipynb  
    Run time - around 1.5 hours  
    script generates following files, which is used in final model building  
        directed_degrees.pkl - degree features for directed contact graph  
   
3. neighbours_features.ipynb  
    Run time - around 12 hours  
    script generates following files, which is used in final model building  
        neigbours_vars_pat_leftover_2.pkl  
        neigbours_vars_sahil_2.csv  
        neigbours_vars_sahil_1.csv  
        degree_2_neighbour_feats.pkl  
          
4. leak_analysis.ipynb  
    Run time - around 1 hours  
    script generates following files, which is used in final model building  
        leak_feature.pkl  
          
5. freq_train_test.ipynb  
    Merges the user features with train and test data and applies frequency encoding on the nodes  
    Run time - around 1.5 hours  
        freq_new_train.pkl - frequency encoded with user features and degree contacts for train  
        freq_new_test.pkl - frequency encoded with user features and degree contacts for test  
        
6. train_script.ipynb  
    Merges all the above set and creates final data for modelling and builds 10 models of LightGBM on that  
    Run time - around 20 hours  (Each model approx 2 hours)  
    For sanity check the final data set should contain 128 columns  
        Saves pickles of all the models  
  
7. test_script.ipynb  
    Creates final test data and final predictions  
    Generates final_sol.csv which is used for final submission  
    
    
    
    
    
    



    
        

    

    
    
