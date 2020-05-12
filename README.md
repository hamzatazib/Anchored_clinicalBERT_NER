# Anchored_clinicalBERT_NER
An anchoring approach to Medical Information Extraction using Clinical BERT Embeddings.

Abstract: Our group was interested in solving the problem of transforming digitized clinical text (e.g., discharge summaries and progress notes) into structured representations of medical concepts with three named entities: medical problems, treatments, and tests. To accomplish this, we created a noisy-labeled dataset by combining information from UMLS terms with discharge summaries from the MIMIC III database and training the open-source clinicalBERT (Alsentzer et al., 2019) for NER on this noisy-labeled dataset to serve as a warm-started BERT model, which we then finetuned for NER on the 2010 i2b2 dataset. We explored two different top layers to perform NER: Linear layer or Bi-LSTM + CRF layer. We also explored how well our model performed using varying levels of the i2b2 data (0%, 20%, 50%, 70%, and 100%) in the final training step to see if gold-labeled data was necessary for producing a reliable medical concept extraction model, showing promising results in how generalizable such a warm start could be.
