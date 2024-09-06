
# Text Clustering and Topic Extraction from COVID-19 Research Papers

## Introduction

In the wake of the COVID-19 pandemic, numerous research articles have been published. This dataset contains information on 10,000 COVID-19 related papers in a CSV file. 

## Objective

With the rapid expansion of COVID-19 research, keeping up with new information is challenging. This project explores whether clustering similar research papers can simplify finding relevant publications and if key topics can be extracted from these clusters.

## Data Preparation

### Text Preprocessing

1. **Language Detection**: Identify and filter out non-English articles using `langdetect`.
2. **Tokenization**: Use spaCy’s `en_core_sci_lg` pipeline for tokenizing and lemmatizing.
3. **Stopwords Removal**: Remove common stopwords.
4. **Punctuation Removal**: Eliminate punctuation marks.

### Feature Extraction

1. **TF-IDF**: Convert preprocessed text to numerical features using the TF-IDF method.
2. **Dimensionality Reduction**: Apply PCA to reduce dimensions while preserving 95% of variance.

## Clustering

1. **K-Means**: Perform clustering with K-Means. Determine optimal cluster count using the Elbow Method.
2. **Evaluation**: Compare K-Means with other clustering methods like Hierarchical and DBSCAN using silhouette, Calinski-Harabasz, and Davies-Bouldin scores.

## Visualization

1. **t-SNE**: Reduce feature dimensions to 2D for visualization of clusters.

## Topic Modeling

1. **LDA**: Extract key topics for each cluster using Latent Dirichlet Allocation (LDA). 
2. **Comparison**: Compare LDA with other topic modeling methods like NMF and LSA.

## Usage

1. Preprocess texts as outlined.
2. Extract features and perform dimensionality reduction.
3. Cluster papers and evaluate clustering methods.
4. Visualize clusters and model topics.

## Requirements

- Python libraries: `pandas`, `nltk`, `spacy`, `sklearn`, `gensim`, `matplotlib`, `seaborn`

