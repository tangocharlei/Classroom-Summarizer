# 🎙️ Audio Transcription, Q&A, and Summarization App

This repository provides a powerful application for audio transcription, question answering (Q&A), and text summarization using state-of-the-art machine learning models. With an intuitive interface powered by **Gradio**, users can transcribe audio, ask questions based on the transcription, and summarize text easily.

---

## ✨ Features

- **Audio Transcription**: Transcribe audio files to text using OpenAI's Whisper model.
- **Question Answering**: Ask questions about the transcribed content with context-aware answers powered by Sentence Transformers and BART.
- **Text Summarization**: Generate concise summaries for large blocks of text or transcriptions using BART.
- **User-Friendly Interface**: An interactive Gradio-based GUI for seamless interaction.

---

## 🛠️ Setup and Installation

Follow these steps to set up the project on your local machine:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/classroom-discussion-summarizer.git
   cd real-time-os-performance-dashboard

2. **Install Dependencies:** Install the required python libraries
   ```bash
   pip install git+https://github.com/openai/whisper.git
   pip install ffmpeg chromadb sentence-transformers transformers gradio

---

## 🚀 Usage

1. **Clone the Repository:**

    Start the Gradio application by executing
   ```bash
   python summarizer+questions.py


2. **Access the interface:**
   
    Open the URL displayed in the terminal (typically http://127.0.0.1:7860) to access the application.


3. **Interact with features:**
   
- **Transcription and Q&A**: Upload an audio file and optionally ask a question about the transcription.
- **Summarization**: Upload an audio file and optionally ask a question about the transcription.

---

## 🔍 How It Works

### 📝 Audio Transcription
1. **Whisper Model**: Converts audio into text with high accuracy.
2. **Chunk Splitting**: Splits transcription into manageable text chunks and stores them in ChromaDB.

### ❓ Question Answering
1. **SentenceTransformer**: Encodes user questions into embeddings.
2. **ChromaDB Query**: Retrieves the most relevant transcription chunks.
3. **BART Model**: Generates answers based on the combined context.

### 🗒️ Text Summarization
   **BART**: Summarizes text into concise and readable content.

---

## 📊 Example Usage

### Transcription and Q&A
1. Upload an audio file.
2. Ask a question, e.g., "What is the main topic of the transcription?".
3. View the transcription and the answer in real-time.

### Summarization
1. Paste a block of text.
2. Click Summarize to generate a concise summary.

---

## 🧑‍💻 Tech Stack

- **Python**: Programming language.
- **Whisper**: Audio transcription.
- **SentenceTransformer**: Question answering.
- **BART**: Text summarization.
- **Gradio**: Interactive UI.
