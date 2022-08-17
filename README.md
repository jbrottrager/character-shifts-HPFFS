# Character Shifts in Harry Potter Fanfiction

This repository provides scripts and data to accompany the Litlab Pamphlet ["Character Shifts in Harry Potter Fanfiction"] (https://www.digitalhumanitiescooperation.de/pamphlet-10-character-shifts-in-harry-potter-fanfiction/) (2022).

 |__ `data/entities`
 
 		|__ `entities.csv`: dictionary of entity names, all variations
   
 		|__ `full_names.csv`: dictionary of entity names, first + second name

 |__ `results`
 
 		|__ `cooccurrences` 
   
 			|__ `cooccurring_words`
    
 				|__ `ffs`: words that occur in sentences shared by two characters in fanfics
     
 				|__ `originals`: words that occur in sentences sharted by two characters in the originals
     
 			|__ `cooccurrences_ffs_count_df_sentences.csv`: adjacency matrix of characters with num of sentences they share (ffs)
    
 			|__ `cooccurrences_ffs_rel_df_sentences.csv`: adjacency matrix of characters with rel num of sentences they share (ffs)
    
 			|__ `cooccurrences_originals_count_df_sentences.csv`: adjacency matrix of characters with num of sentences they share (originals)
    
 			|__ `cooccurrences_originals_rel_df_sentences.csv`: adjacency matrix of characters with rel num of sentences they share (originals)
    
 			|__ `freq_names_ffs.csv`: frequency of entity names in each fanfic + relative frequency over all fanfics
    
 			|__ `freq_names_originals.csv`: frequency of entity names in each original novel + relative frequency over all novels
    
 		|__ `vector_models`
   
 			|__ `modelHPFFsD_vectors.kv`: best vector model for fanfics
    
 			|__ `modelHPoriginalsD_vectors.kv`: best vector model for the originals
    
  |__ `scripts`
  
  		|__ `01_generaliseEntities.ipynb`
    
  		|__ `02_characterCooccurrences.ipynb`
    
  		|__ `03_checkCharacterNames.ipynb`
    
  		|__ `04_freqDist.ipynb`
    
  		|__ `05_Word2Vec.ipynb` 
    
  		|__ `06_modelEvaluation.ipynb`
    
  		|__ `07_shiftsWithResiduals.ipynb`
    
  		|__ `08_countFrequenciesAll.ipynb` 
    
  		|__ `09_BAWLcluster.ipynb`
    
  		|__ `10_emotionalProfiles.ipynb` 
