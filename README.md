# MoMagic — AI-Powered Meeting Minutes Generator

Automatically converts meeting audio into professional, structured Minutes of Meeting using AI.

## Overview

Preparing Minutes of Meeting manually is time-consuming, and important decisions or action items are often missed during note-taking — especially in long meetings. **MoMagic** solves this by automatically transcribing, analyzing, and summarizing meeting audio into a clean, professional report, with no manual effort required beyond uploading the recording.

## Key Features

- 🎙️ **Speech-to-text transcription** using Whisper AI, robust to multilingual and noisy audio
- 🌐 **Multilingual meeting support** with automatic language detection
- 🧠 **AI-based summarization** (via OpenRouter/GPT) generating structured Meeting Summary, Key Decisions, Action Items, and Important Discussion Points
- 🔑 **Keyword extraction** to surface key discussion topics
- 💬 **Sentiment analysis** using TextBlob
- 📄 **Professional report generation** — downloadable PDF and TXT output via ReportLab
- 🖥️ **Simple web interface** built with Gradio — no setup needed for end users

## How It Works

1. **Audio Upload** — User uploads a meeting recording through the Gradio interface
2. **Speech-to-Text** — Whisper AI converts the audio into an accurate transcript
3. **Transcript Cleaning** — Removes noise, symbols, and formatting issues for readability
4. **Language Detection** — Automatically identifies the language used
5. **Speaker Identification** — Structures the transcript speaker-wise
6. **Keyword Extraction** — Surfaces key terms and topics using Regex & Counter
7. **AI Summarization** — Generates structured Minutes of Meeting via an LLM (OpenRouter)
8. **Report Generation** — Outputs a polished, downloadable PDF/TXT report

## Tech Stack

| Category | Technology |
|---|---|
| Language | Python |
| Speech Recognition | Whisper AI |
| AI Summarization | OpenRouter / GPT model |
| Frontend | Gradio |
| NLP | TextBlob (sentiment analysis) |
| Report Generation | ReportLab |
| Keyword Processing | Regex & Counter |
| Development Platform | Google Colab |

## Sample Output

**Upload interface:**

![Upload Interface](Upload%20interface.jpeg)

**Live transcription:**

![Live Transcription](Live%20transcription.jpeg)

**AI-generated structured minutes:**

![Generated Minutes](AI-generated%20structured%20minutes.jpeg)

**Final professional PDF report:**

![PDF Report](Final%20professional%20PDF%20report.jpeg)

## Setup

This notebook was built and run on Google Colab.

1. Open `Momagic.ipynb` in Google Colab
2. Replace `YOUR_API_KEY_HERE` with your own OpenRouter API key
3. Run all cells — Gradio will launch a shareable web interface
4. Upload a meeting audio file and generate your Minutes of Meeting

## Status

Open to feedback and improvements.
