# Character Shifts in Harry Potter Fanfiction

This repository provides scripts and data to accompany the Litlab Pamphlet ["Character Shifts in Harry Potter Fanfiction"](https://www.digitalhumanitiescooperation.de/pamphlet-10-character-shifts-in-harry-potter-fanfiction/) (2022). 

- `data/entities`
  * `entities.csv`: dictionary of entity names, all variations
  * `full_names.csv`: dictionary of entity names, first + second name
- `results`
  * `cooccurrences` 
    * `cooccurring_words`
      * `ffs`: words that occur in sentences shared by two characters in fanfics
      * `originals`: words that occur in sentences shared by two characters in the originals
    * `cooccurrences_ffs_count_df_sentences.csv`: adjacency matrix of characters with num of sentences they share (ffs)
    * `cooccurrences_ffs_rel_df_sentences.csv`: adjacency matrix of characters with rel num of sentences they share (ffs)
    * `cooccurrences_originals_count_df_sentences.csv`: adjacency matrix of characters with num of sentences they share (originals)
    * `cooccurrences_originals_rel_df_sentences.csv`: adjacency matrix of characters with rel num of sentences they share (originals)
    * `freq_names_ffs.csv`: frequency of entity names in each fanfic + relative frequency over all fanfics
    * `freq_names_originals.csv`: frequency of entity names in each original novel + relative frequency over all novels
- `vector_models`
  * `modelHPFFsD_vectors.kv`: best vector model for fanfics
  * `modelHPoriginalsD_vectors.kv`: best vector model for the originals
- `scripts`
  * `01_generaliseEntities.ipynb`: replacing name variations with an entity name
  * `02_characterCooccurrences.ipynb`: finding co-occurrences of characters in sentences
  * `03_checkCharacterNames.ipynb`: calculating frequency distributions for entity names + Figures 4.1-4.2
  * `04_freqDist.ipynb`: identifying words that occur in sentences shared by two characters
  * `05_Word2Vec.ipynb`: creating wor2vec models
  * `06_modelEvaluation.ipynb`: evaluating word2vec models + Figures 6.8-6.9
  * `07_shiftsWithResiduals.ipynb`: comparing frequency of character pairings with residuals + Figures 5.3-5.6
  * `08_countFrequenciesAll.ipynb`: calculating frequencies for emotion words
  * `09_BAWLcluster.ipynb`: clustering emotion words in vector models
  * `10_emotionalProfiles.ipynb`: creating emotional profiles + Figures 6.10-6.15
