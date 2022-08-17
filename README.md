# Character Shifts in Harry Potter Fanfiction

This repository provides scripts and data to accompany the Litlab Pamphlet ["Character Shifts in Harry Potter Fanfiction"](https://www.digitalhumanitiescooperation.de/pamphlet-10-character-shifts-in-harry-potter-fanfiction/) (2022). 

- `data/entities`
  * `entities.csv`: dictionary of entity names, all variations
  * `full_names.csv`: dictionary of entity names, first + second name
- `results`
  * `cooccurrences` 
    * `cooccurring_words`
      * `ffs`: words that occur in sentences shared by two characters in fanfics
      * `originals`: words that occur in sentences sharted by two characters in the originals
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
  * `01_generaliseEntities.ipynb`
  * `02_characterCooccurrences.ipynb`
  * `03_checkCharacterNames.ipynb`
  * `04_freqDist.ipynb`
  * `05_Word2Vec.ipynb` 
  * `06_modelEvaluation.ipynb`
  * `07_shiftsWithResiduals.ipynb`
  * `08_countFrequenciesAll.ipynb` 
  * `09_BAWLcluster.ipynb`
  * `10_emotionalProfiles.ipynb`
