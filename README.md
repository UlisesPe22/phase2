## Summary of Analysis
This analysis aimed to identify the most relevant topics within a civic complaints dataset, in which real-world Indian citizens reported issues concerning public services and infrastructure. To accomplish this task, two distinct Pipelines were implemented: 
•	Pipeline A: encoded every complain with SBERT, reduced the embeddings with UMAP, clustered them with HDBSCAN, and extracted topics using C-TF-IDF and KeyBERT.
•	Pipeline B: vectorized each complain text with TF-IDF, reduced the vectorial space dimensions with LSA, find clusters with K-Means, and extract semantic topics
## Repository Layout
The data analysis was made with Jupyter Notebooks, and it has been organized in the following files:
•	Cleaning_Original_Dataset: In this his file the original dataset is processed, and the cleaned data frames used to build both pipelines are obtained.
•	Sbert_Vectorization: This notebook performs the vectorization of the preprocessed complaint texts using SBERT. The resulting 768-dimensional embeddings are saved to the data folder to be reused in Pipeline A.
•	Data: This folder holds all the used data frames and the embeddings produced by Sbert_Vectroization file. 
•	Pipeline_A_SBERT_UMAP_HDBSCAN: This notebook contains the full implementation of Pipeline A, including dimensionality reduction, clustering, topic extraction, and the discussion of results.
•	Pipeline_B_TFIDF_LSA_KMEANS: This notebook contains the full implementation of Pipeline B, applying TF-IDF vectorization, LSA dimensionality reduction and K-Means clustering. Furthermore, it has topic extraction and the discussion of results.
All notebooks include Markdown cells where results and process are discussed and explained.
