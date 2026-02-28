# Restaurant Query Agent

This directory contains the implementation of an AI-powered FAQ chatbot for "The Daily Dish" restaurant. The chatbot is designed to answer customer questions by retrieving information from a provided FAQ PDF and generating friendly, accurate responses.

## Files Overview

### 1. `bucket.fud.ipynb`
- **Type:** Jupyter Notebook
- **Purpose:** Main notebook for building, testing, and demonstrating the restaurant FAQ chatbot.
- **Contents:**
  - Project overview and workflow description.
  - Step-by-step code for:
    - Extracting text from the FAQ PDF.
    - Splitting the text into question-answer pairs.
    - Vectorizing questions for similarity search.
    - Retrieving the most relevant answer to a user query.
    - Example usage and output.
  - Instructions for required Python packages (`pypdf`, `scikit-learn`, `nltk`).
  - Code is modularized for easy understanding and extension.

### 2. `The_Bucket.fud_FAQ.pdf` (expected, not included)
- **Type:** PDF Document
- **Purpose:** The FAQ document containing questions and answers about the restaurant's services, menu, reservations, and more.
- **Note:** This file should be placed in the same directory as the notebook. If not present, update the path in the notebook or download from the provided source link in the notebook.

## How It Works

1. **Query Understanding:**
   - The user's question is interpreted to extract intent and keywords.
2. **Document Retrieval:**
   - The FAQ PDF is searched for the most relevant answer using TF-IDF and cosine similarity.
3. **Memory Phase:**
   - (Planned/Optional) Stores and recalls conversation context for personalized responses.
4. **Response Generation:**
   - The best-matching answer is cleaned and presented to the user.

## Getting Started

1. Install required packages:
   ```python
   !pip install pypdf scikit-learn nltk
   ```
2. Place the FAQ PDF in this directory.
3. Open and run the notebook `bucket.fud.ipynb`.

## Customization
- You can update the FAQ PDF or modify the code to handle different document formats or more advanced conversation memory.

## Contact
For questions or suggestions, please contact the project maintainer or open an issue in your repository.
