# CSE508_Winter2024_A2_MT23045

# Image Feature Extraction:

**Approach:** Utilized the ResNet50 pre-trained model to extract features from images. Employed basic image preprocessing techniques such as resizing, flipping, and enhancing brightness, contrast, and color.

**Methodology:** Created functions for image preprocessing, downloading, and extracting features. Used the ResNet50 model to extract features from images and normalized them.

**Assumptions:** Assumed that ResNet50's pre-trained weights would capture meaningful image features relevant to similarity calculation.

**Results:** Extracted image features were normalized and saved using pickle for further use in image retrieval tasks.

# Text Preprocessing and TF-IDF Calculation:

**Approach:** Employed Natural Language Toolkit (NLTK) for text preprocessing and Term Frequency-Inverse Document Frequency (TF-IDF) calculation for textual data.

**Methodology:** Preprocessed text data by lower-casing, removing ellipses, stopwords, punctuation, stemming, and lemmatization. Calculated TF-IDF scores to represent the importance of words in reviews.

**Assumptions:** Assumed that TF-IDF scores would adequately capture the significance of words in reviews for similarity calculation.

**Results:** Generated TF-IDF scores for textual data and saved them using pickle for similarity calculation in review retrieval tasks.

# Image and Text Retrieval:

**Approach:** Implemented image and text retrieval based on cosine similarity.

**Methodology:** Calculated cosine similarity between input image features and all image features, as well as between input TF-IDF scores and all TF-IDF scores. Combined image and text retrieval results for comprehensive similarity ranking.

**Assumptions:** Expected that similar images and reviews would have high cosine similarity scores.

**Results:** Provided top similar images and reviews along with their cosine similarity scores. Also, conducted combined retrieval to rank pairs based on composite similarity scores.

Overall, the approach involved extracting meaningful features from images and text, calculating similarity scores using cosine similarity, and conducting retrieval tasks based on these scores. The methodology was structured, leveraging pre-trained models and standard techniques for feature extraction and similarity calculation. Assumptions were made regarding the effectiveness of pre-trained models and TF-IDF scores in capturing relevant information. The results demonstrated the effectiveness of the approach in retrieving similar images and reviews based on input queries.
