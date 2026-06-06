# Dune NLP Analysis

NLP research project based on Frank Herbert's novel *Dune*.  
The goal of this project is to explore basic NLP techniques on a full-length literary text and extract meaningful structure from it.

---

## Project Overview

In this project, I apply fundamental NLP methods to analyze a large English-language fiction text.  
The focus is on text structure, character analysis, and topic modeling.

---

## Work Performed

- Loaded and preprocessed the original English text (lowercasing, punctuation removal, stopwords filtering)
- Extracted most frequent words in the entire text
- Split the book into chapters using epigraphs (since the original text does not contain explicit chapter numbering)
- Analyzed most frequent words per chapter
- Estimated character importance based on mention frequency
- Extracted most unique words for each chapter
- Applied TF-IDF analysis to chapters
- Performed topic modeling using LDA
- Built character-based text representations using TF-IDF
- Created character embeddings using SBERT
- Visualized character relationships using t-SNE

---

## Technologies Used

- Python
- pandas
- numpy
- matplotlib
- re
- collections (Counter)
- spaCy
- scikit-learn:
  - TF-IDF Vectorizer
  - CountVectorizer
  - LDA (Latent Dirichlet Allocation)
  - PCA
  - t-SNE
  - cosine similarity
- sentence-transformers (SBERT)

---

## Key Insights

- Character analysis with and without other character names produces different semantic perspectives:
  - With names → social and relational character portrait
  - Without names → behavioral and thematic character description
- Topic modeling on raw text reveals high-level narrative structure around the protagonist
- Removing the protagonist's name from the corpus allows separation of independent narrative threads:
  - personal life
  - political and social intrigue
  - desert/ecological theme
  - espionage and strategic conflicts

---

## Project Structure

NLP-Dune/
│
├── dune_analysis.ipynb        # main research notebook
├── README.md
├── dune.txt                   # raw book text (English version)
└── characters_semantic_map.png  # character relationship visualization
