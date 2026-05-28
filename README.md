# Characteristics of the Topological Structure of Language as Observed in Non-Standard Speakers


The project investigates whether second-language learners and heritage speakers position themselves differently relative to persistent semantic structures (*H₁ holes*) in the embedding space of a language. The study combines methods from:

* computational linguistics,
* second language acquisition (SLA),
* distributional semantics,
* and topological data analysis (TDA).

Using persistent homology computed over Word2Vec embedding spaces, the project identifies stable semantic holes in English and Russian and measures how different writer populations relate to those structures.

## Research Questions

* Do native and learner writing differ in their relation to persistent semantic holes?
* Can semantic topology reveal traces of cross-linguistic transfer?

## Main Components

### Data

The experiments use multiple English and Russian corpora, including:

* REALEC
* BAWE
* PERSUADE
* CoRST
* RULEC / RLC
* large literary and academic reference corpora

### Embedding Spaces

Reference semantic spaces are constructed using:

* Word2Vec CBOW embeddings
* cosine-distance semantic geometry
* large-scale lemmatized corpora

### Persistent Homology

The project computes persistent first-order homology (*H₁*) using:

* Vietoris–Rips filtrations
* Ripserer.jl
* adaptive patch-based topology computation

### Feature Extraction

For each essay, the pipeline computes multiple hole-distance feature groups, including:

* distance to hole centers,
* minimum contour distance,
* maximum contour distance,
* nearest-hole preference distributions.

### Statistical Analysis

The experiments use:

* Kolmogorov–Smirnov tests,
* Benjamini–Hochberg FDR correction,
* Cohen’s *d* effect sizes,
* distributional visualization and exploratory analysis.


## Methodological Notes

* All corpora were lemmatized and normalized before embedding training.
* Persistent homology was computed on reference corpora rather than directly on learner corpora.
* Hole filtering combines persistence thresholds with semantic diameter filtering based on WordNet and RuWordNet.
* The study focuses on semantic topology rather than classification accuracy alone.

## Technologies

* Python
* Julia
* Google Colab
* gensim
* Ripserer.jl
* spaCy
* Natasha
* pandas
* NumPy
* scikit-learn

## Author

Alexandra Pogozheva
National Research University Higher School of Economics (HSE University)

