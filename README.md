# RAG-Based AI System 

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline that converts video lectures into searchable knowledge and answers user queries using semantic similarity.

The system processes video files, transcribes audio using Whisper, generates embeddings, and retrieves the most relevant content for a given query.



## 🚀 Features

- Convert video files to audio (MP3)
- Transcribe audio using Whisper
- Store transcripts in structured JSON format
- Preprocess and chunk text data
- Generate and store embeddings using Joblib
- Perform semantic search using cosine similarity
- Lightweight and fully local (no paid APIs required)



## 🧠 Tech Stack

- *Python 3.9+*
- *Whisper (Speech-to-Text)*
- *NumPy & Pandas*
- *Scikit-learn (Cosine Similarity)*
- *Joblib (Embedding Storage)*
- *FFmpeg (Video/Audio Processing)*
-  *bge-m3(for embedding)
-  *llama3.2(for LLM output/ generated response)
