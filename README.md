# Development of a microbiome corpus with >100k annotated bacterial, fungal and archaeal entities
A Natural language processing project done as part of my MRes degree which involves named entity recognition(NER) and training deep learning models, Here are some of the files included here : 

- NCBI-dictionary : Includes the code to clean and process the NCBI data into one dataset as a dictionary which will include each microbiome, their kingdom and their taxonomic rank. 
- Annotation_pipeline : Includes the pipeline which will use string matching with the dictionary data and some rule-based methods to annotate all the microbiome in a publication. 
- BioBert_input : Converts the annotated publication into the format needed by biobert. 

# Methods: 
The study introduces a newly developed pipeline to automatically annotate microbial entities (bacteria, archaea, fungi) in biomedical publications. This pipeline has been developed through string matching and rule-based annotation. A taxonomic rank dictionary has also been created to aid the string matching and detect each entity`s taxonomic rank and kingdom. Furthermore, a BioBERT-BiLSTM deep learning model was trained to detect all microbiome entities. This model was tested on a manually annotated test set.

# Results:
The automatic annotation has been tested against a manually annotated test set and has achieved a state-of-the-art performance of an F1-score of 0.975 (precision = 0.9847, recall = 0.9664). The pipeline can annotate a full-text publication in 2-4 seconds. The corpus contains 112,690 annotations of bacteria, fungi and archaea from subkingdoms to species level. The deep learning model achieved an F1-score of 0.9599 (precision = 0.9771, recall = 0.9597) on the test data.

# Conclusion: 
The results from automatic annotation have showed that the pipeline introduced in this study is very precise and it can predict the taxonomic rank and kingdom of all microbiota in a biomedical publication quickly. Moreover, the BioBERT-BiLSTM model was trained on the annotated files and has also achieved state-of-the-art results.

