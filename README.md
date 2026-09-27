# SmartCampus NLP Assistant

NLP-Based Natural Language Query Retrieval System for Campus FAQs

## Overview

SmartCampus NLP Assistant is an NLP-based FAQ retrieval application.
It allows users to enter campus-related questions in natural language
and retrieves the most relevant stored FAQ using TF-IDF and cosine similarity.

## Technologies

- Python
- Pandas
- scikit-learn
- Streamlit
- CSV

## How It Works

User Query
↓
Text Processing
↓
TF-IDF Vectorization
↓
Cosine Similarity
↓
Highest Similarity FAQ
↓
Answer + Category + Similarity Score

## Dataset

The project uses an illustrative/synthetic campus FAQ dataset created
for academic demonstration. It is not official university data.

## Run Locally

Install dependencies:

pip install -r requirements.txt

Run the application:

python -m streamlit run app.py

The application will open at the local Streamlit address.

## Testing

Representative test queries include:

- how do I get my admit card
- when can I use the library
- how to join hostel
- placement registration

The recorded similarity scores are documented in `test_results.csv`.

## Limitations

The current system uses lexical TF-IDF retrieval and may have difficulty
with synonyms and semantic paraphrases.

## Future Scope

- Sentence embeddings
- Multilingual retrieval
- Verified institutional knowledge base
- Authentication and analytics
- Optional RAG/LLM layer
