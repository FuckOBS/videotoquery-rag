🎥 RAG-Based Video Question Answering System

🎯 Problem Statement

Educational video lectures and online courses are often long and unstructured. Learners frequently need to revisit specific concepts, but finding the exact moment where a topic is explained requires rewatching large portions of the video, which is time-consuming and inefficient.

✅ Solution

This project builds a Retrieval-Augmented Generation (RAG) system that converts video lectures into searchable knowledge.

Users can ask natural language questions and instantly retrieve the most relevant explanation, along with the corresponding video segment and timestamp, using semantic search.

🧠 End Goal (Core Use-Case)
Enable semantic search and question answering over long educational videos, allowing users to locate exact explanations without rewatching entire lectures.

Target Users
Students learning from online courses or YouTube tutorials
Self-learners revising specific concepts
Educators managing large lecture repositories

🚀 Key Features
Convert video lectures to audio using FFmpeg
Transcribe audio to text using Whisper
Store transcripts in structured JSON format with timestamps
Chunk transcripts into semantically meaningful segments
Generate multilingual embeddings using bge-m3 (Ollama)
Perform semantic retrieval using cosine similarity
Generate context-aware answers using LLaMA 3.2
Fully local pipeline (no paid APIs required)

🏗️ System Architecture

Video → Audio → Transcription → Chunking → Embeddings → Vector Search → RAG Answer

Each component is designed to support the final goal of accurate, timestamp-aware retrieval from long-form video content.

🛠️ Tech Stack
Core Language
Python 3.9+
Speech-to-Text
OpenAI Whisper (small model)
Embeddings
Ollama
bge-m3 (multilingual embedding model)
Retrieval & Similarity
NumPy
Scikit-learn (Cosine Similarity)
Joblib (Embedding storage)
LLM for Answer Generation
LLaMA 3.2 (via Ollama)
Media Processing
FFmpeg

📂 Project Workflow
Convert videos to audio files
Transcribe audio using Whisper
Store transcripts with timestamps in JSON format
Chunk transcripts into manageable semantic units
Generate embeddings using bge-m3
Perform semantic similarity search for user queries
Use retrieved context to generate answers via LLaMA

📌 Example Use Case
User Query:
“Where is the HTML media player explained?”
System Output:
Relevant explanation text
Corresponding video title
Exact timestamp where the concept is discussed

📈 Future Improvements
FAISS integration for scalable vector search
Web-based UI (Streamlit / React)
Multi-video and multi-course indexing
Metadata-based filtering (topic, duration, chapter)
Answer summarization with confidence scoring

💡 Why This Project Matters
This system demonstrates how RAG can be applied beyond documents to real-world multimedia data.

The same architecture can be extended to:
Corporate training videos
MOOCs and e-learning platforms
Internal knowledge bases
Recorded meetings and webinars

👤 Author
Gursimran
AI / Data Science Enthusiast
