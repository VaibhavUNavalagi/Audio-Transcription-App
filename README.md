# 🎙️ Audio Transcription & Summarization App (Whisper + IBM Watson + Gradio)

## 📌 Introduction

Imagine attending a business meeting where every discussion is automatically transcribed and summarized with key points highlighted. This project implements an AI-powered application that converts speech into text using **OpenAI Whisper**, analyzes and summarizes the content using **IBM Watson LLMs**, and provides a clean, interactive interface using **Gradio**.

The application demonstrates an end-to-end **speech-to-text and language understanding pipeline**, combining modern AI models with a user-friendly web interface.

---

## 🎯 Learning Objectives

By completing this project, you will be able to:

- Build speech-to-text applications using OpenAI Whisper  
- Work with Large Language Models (LLMs) for text generation and summarization  
- Integrate IBM Watson foundation models using LangChain  
- Design interactive web interfaces using Hugging Face Gradio  
- Develop complete AI pipelines combining speech, language, and UI components  

---

## 🛠️ Tech Stack

- **Speech Recognition:** OpenAI Whisper  
- **Language Models:** IBM Watsonx (LLaMA 3)  
- **Frameworks & Libraries:**  
  - Hugging Face Transformers  
  - LangChain  
  - Gradio  
- **Programming Language:** Python  
- **System Dependency:** FFmpeg  

---

## 📂 Project Structure

```text
Audio-Transcription-App/
├── hello.py                 # Gradio quickstart demo
├── simple_speech2text.py    # Basic Whisper-based transcription script
├── speech2text_app.py       # Audio transcription Gradio app
├── simple_llm.py            # Text generation using IBM Watson LLM
├── speech_analyzer.py       # Full pipeline: STT + LLM summarization
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
```

---

## ⚙️ Environment Setup
### 1️⃣ Create and activate a virtual environment
```bash
pip3 install virtualenv
virtualenv my_env
source my_env/bin/activate
```
### 2️⃣ Install required libraries
```bash
pip install transformers==4.36.0 \
            torch==2.1.1 \
            gradio==5.23.2 \
            langchain==0.0.343 \
            ibm_watson_machine_learning==1.0.335 \
            huggingface-hub==0.28.1
```
### 3️⃣ Install FFmpeg (required for audio processing)
```bash
sudo apt update
sudo apt install ffmpeg -y
```
---

## 🔊 Step 1: Speech-to-Text using OpenAI Whisper

A basic transcription script uses the openai/whisper-tiny.en model to convert audio files into text.
```bash
python3 simple_speech2text.py
```
## 🌐 Step 2: Audio Transcription Web App (Gradio)

An interactive Gradio application allows users to upload .mp3 audio files and receive transcribed text instantly.
```bash
python3 speech2text_app.py
```
#### Features:

Upload audio files
Automatic transcription using Whisper
Real-time web interface

## 🤖 Step 3: Text Generation with IBM Watson LLM

A standalone script demonstrates text generation using LLaMA 3 via IBM Watsonx.
```bash
python3 simple_llm.py
```
Key parameters such as temperature and maximum tokens are configured to control output quality and creativity.

## 🔗 Step 4: End-to-End Speech Analyzer (STT + LLM)

The final application integrates:

Speech-to-Text using Whisper
Prompt-based summarization using IBM Watson LLM
Gradio-based UI for interaction

```bash
python3 speech_analyzer.py
```
Workflow:

1. User uploads an audio file
2. Whisper transcribes speech into text
3. Transcription is passed to an LLM with a structured prompt
4. Key points and summaries are generated
5. Results are displayed in the web interface

---

## 🧪 Results

- Accurate speech transcription from audio recordings  
- Context-aware summarization and key-point extraction  
- Interactive and user-friendly web interface  
- Robust end-to-end AI pipeline  

---

## 💡 Use Cases

- Business meeting transcription and summarization  
- Lecture and seminar analysis  
- Educational content processing  
- Research and AI prototyping  
- Accessibility tools  

---

## 📈 Conclusion

This project provides hands-on experience with modern AI systems for speech recognition and language understanding. By combining **OpenAI Whisper**, **IBM Watson LLMs**, and **Gradio**, the application demonstrates how multiple AI components can be orchestrated into a cohesive, real-world solution.

---

## 👤 Author

**Vaibhav U Navalagi**














