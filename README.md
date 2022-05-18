# **How to run our program:**

### - Download the dataset from [IMDb Reviews](https://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz) 
### - Move the downloaded tar.gz file into your desired directory where you will be accessing it from. To make this step easier, we recommend using desktop directory.
### - Open a terminal where you stored the tar.gz file. Please double check that the terminal is opened on the correct directory. If not, navigate to the directory              where you stored the tar.gz file by using 'cd' command. Run the following command in your terminal:
   - gunzip -c aclImdb_v1.tar.gz | tar xopf -
   - cd aclImdb && mkdir movie_data
   - for split in train test; do for sentiment in pos neg; do for file in $split/$sentiment/*; do cat $file >> movie_data/full_${split}.txt; echo >>                             movie_data/full_${split}.txt; done; done; done;

### - Locate the following code in the program & replace the URL with the location of your full_train.txt and full_test.txt files in your desktop.
   ```python
   for line in open('C:/Users/kurti/Desktop/aclImdb/movie_data/full_train.txt', encoding='utf-8'):
    reviews_train.append(line.strip())
    
   reviews_test = []
   for line in open('C:/Users/kurti/Desktop/aclImdb/movie_data/full_test.txt', encoding='utf-8'):
    reviews_test.append(line.strip())
   ```
### - Install NLTK (pip install nltk), Scikit (pip install -U scikit-learn)
### - Run the program & enjoy. 

created by: ![follow me](https://img.shields.io/github/followers/kurtina09?label=Kurtina09&style=social) _
![follow me2](https://img.shields.io/github/followers/illiquid47?label=illiquid47&style=social)
