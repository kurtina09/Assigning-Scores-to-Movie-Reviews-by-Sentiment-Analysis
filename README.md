# Assigning Scores to Movie Reviews by Sentiment Analysis

# How to run our program:

1. Download the dataset from IMDb Reviews by clicking the link below: 
    (https://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz) 
2. Unpack and Merge the dataset
    a. Move the downloaded tar.gz file into your desired directory where you will be accessing it from. To make this step easier, we recommend using desktop directory
    b. Open a terminal where you stored the tar.gz file. Please double check that the terminal is opened on the correct directory. If not, navigate to the directory              where you stored the tar.gz file by using 'cd' command. 
    c. gunzip -c aclImdb_v1.tar.gz | tar xopf -
    d. cd alcImdb && mkdir movie_data
    e. for split in train test; do for sentiment in pos neg; do for file in $split/$sentiment/*; do cat $file >> movie_data/full_${split}.txt; echo >>                             movie_data/full_${split}.txt; done; done; done;
