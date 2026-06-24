# TextMind AI

An AI-powered text summarization platform built using FastAPI and Hugging Face Transformers. The application leverages the T5 Transformer architecture to generate concise and meaningful summaries from long-form text.

## Features

* Abstractive Text Summarization
* FastAPI Backend
* Interactive Web Interface
* Hugging Face Transformers Integration
* T5 Transformer Architecture
* Cross-Platform Support (CPU, CUDA, Apple Silicon)

## Tech Stack

* Python
* FastAPI
* Hugging Face Transformers
* PyTorch
* HTML
* CSS
* JavaScript

## Project Structure

```text
TextMind-AI/
│
├── app.py
├── index.html
├── requirements.txt
├── README.md
├── Text_Summarizer.ipynb
└── screenshots/
```

## How It Works

1. User enters text in the web interface.
2. FastAPI receives the request.
3. Text is preprocessed and tokenized.
4. T5 Transformer generates a summary.
5. Summary is returned and displayed on the frontend.

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/TextMind-AI.git
cd TextMind-AI
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Model Setup

The trained model files are not included in this repository due to GitHub file size limitations.

You can download a T5 model directly from Hugging Face:

```python
from transformers import T5ForConditionalGeneration, T5Tokenizer

model = T5ForConditionalGeneration.from_pretrained("t5-small")
tokenizer = T5Tokenizer.from_pretrained("t5-small")
```

Or place your trained model files inside:

```text
saved_summary_model/
```

## Running the Application

Start the FastAPI server:

```bash
uvicorn app:app --reload
```

Open your browser:

```text
http://127.0.0.1:8000
```

## Dataset

This project was developed using the SAMSum Dataset, a dialogue summarization dataset designed for conversational text summarization tasks.

## Future Improvements

* PDF Summarization
* Document Upload Support
* Multiple Transformer Models
* ROUGE Score Evaluation
* Model Deployment on Hugging Face Spaces

## Screenshots

Add screenshots of:

* Home Page
* Generated Summary Page

## Author

**Siddhanth Singh**

B.Tech Computer Science & Engineering

Interested in AI/ML, NLP, Competitive Programming, and Backend Development.
