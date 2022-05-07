# Lovecraft-Digital-Analytical-Edition
 A digital analytical edition of lovecrafts works for academic use. Contained in the data folder are all of HP Lovecraft's short stories and poetry.  

## Manifest  

### Data/Code Provenance
All short stories came from the github repo [lovecraftcorpus](https://github.com/RyanDoesMath/lovecraftcorpus)  
All the poetry was copied from www.hplovecraft.com.  
Many portions of code in this repository are copied from the [DS5001 github repo](https://github.com/ontoligent/DS5001-2022-01/blob/main/lib/hac2.py).  

### Data File's and File structure  
All data files are either text files or csv for portability.  
The processed data files can be found in data/output/  
The raw short stories are kept in data/short_stories/  
The poems are kept in data/poems/

### File Dictionary
The CORPUS file contains the entire work broken down by title/sentence/token. The tokens are tagged for part of speech and numbered should you need it.  
The LIB file contains the filepath for each title, the probable date of completion (any decisions about uncertain dates are tracked in the F0_to_F4 jupyter notebook), and the literary format (short story or poem).  
The TOKENS file is deprecated and should be removed in a future pull request as it's function is taken over by CORPUS.  
The VOCAB table contains a large amoutnt of information about each term that appears in the corpus including how many times it appears, how long it is, its stem, probability, typical part of speech, and tfidf mean and max among other things.
RAW is a file that contains the totally unprocessed text in case you don't wish to deal with all the individual text files.  
BOW is a bag of words file. I highly reccomend creating your own with your own parameters from the CORPUS file for any specific use case.  
The SENTIMENT file contains the NRC lexicon based sentiment analysis for each title.  
PCA_COMPS, PCA_DCM, and PCA_THETA are all files associated with PCA analysis. For a better explaination of what these are, read [this](https://github.com/ontoligent/DS5001-2022-01/blob/main/M07_FeaturesAndComponents/M07_01_PCA-REVISED.ipynb) jupyter notebook.
