# Gemini Multimodal App

A collection of multimodal AI applications built with Google Gemini and related models for text, image, and video understanding. Includes a chatbot with vision capabilities and multiple video analysis/commentary generation pipelines.

## Features

- **Multimodal Chatbot** -- Text and image chat using Gemini Pro and Gemini Pro Vision via Gradio
- **Video Summarization** -- Upload and summarize videos using Gemini 1.5 Flash
- **Video Commentary Generation** -- Extract frames from video, caption them with BLIP, generate sports commentary via GPT-3.5 Turbo, and convert to speech with gTTS
- **Vertex AI Integration** -- Video analysis using Google Vertex AI Gemini models

## Tech Stack

- **Language:** Python
- **AI Models:** Google Gemini (Pro, Pro Vision, 1.5 Flash), Salesforce BLIP, OpenAI GPT-3.5 Turbo
- **Frameworks:** Google Generative AI SDK, Vertex AI SDK, Hugging Face Transformers, PyTorch
- **Web Interface:** Gradio
- **Video Processing:** OpenCV, MoviePy
- **Text-to-Speech:** gTTS
- **Vision:** Google Cloud Vision API

## Setup / Installation

```bash
git clone https://github.com/bnarasimha21/gemini-multimodal-app.git
cd gemini-multimodal-app
pip install -r requirements.txt
```

### Environment Variables

```bash
export GOOGLE_API_KEY="your-google-api-key"
export OPENAI_API_KEY="your-openai-api-key"       # For video_to_commentary.py
```

## Usage

### Multimodal Chatbot (Text + Image)

```bash
python app.py
```

Opens a Gradio interface where you can chat with text, upload images, and get AI-generated responses using Gemini Pro / Gemini Pro Vision.

### Video Summarization with Gemini

```bash
python video.py
```

Uploads a video to the Gemini API and generates a text description of its contents.

### Video-to-Commentary Pipeline

```bash
python video_to_commentary.py
```

Extracts frames from a video, generates captions with BLIP, creates sports commentary using GPT-3.5 Turbo, and saves audio commentary as MP3 files.

### Vertex AI Video Summarization

```bash
python gemini_video_summarization.py
```

Uses Google Vertex AI to analyze and describe video content.

## License

MIT
