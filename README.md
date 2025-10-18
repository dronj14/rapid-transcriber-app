# ⚡ Rapid Script Transcriber (Gemini 2.5 Flash)

A fast, single-file web application for transcribing audio and video files using the **Gemini 2.5 Flash API**.

This tool is designed for speed and reliability, featuring structured output (JSON schema) to ensure accurate timecodes and speaker segmentation, and a tight **8MB file size limit** to prevent API timeouts.

## ✨ Features

* **🎙️ Accurate Transcription:** Leverages the power of the multimodal Gemini 2.5 Flash model.
* **👥 Speaker Segmentation:** Automatically inserts speaker labels (e.g., Speaker A:, Speaker B:).
* **⏱️ Integrated Audio Player:** Includes a full-width audio player placed directly above the editable transcript for easy review and correction with time reference.
* **💾 Flexible Downloads:** Export the final transcript as a plain **TXT** file or a timed **SRT** subtitle file.
* **✅ Self-Contained:** The entire application is a single `index.html` file—no backend required.

## 🚀 Live Demo (GitHub Pages)

You can try the live application here:

> **[Open Rapid Script Transcriber](https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/)**
> (Replace the URL above with your actual GitHub Pages link)

## 🛠️ Setup and Installation

Since this is a single-file application, deployment is straightforward.

### 1. Acquire a Gemini API Key

1.  Get your API key from **[Google AI Studio](https://ai.google.dev/gemini-api/docs/api-key)**.
2.  Ensure you have enabled billing on your Google Cloud Project to use the API (transcription is a paid, but low-cost, operation).

### 2. Update the `index.html` file

You must replace the placeholder API key in the `index.html` file with your actual key.

Open your local `index.html` file (or edit it directly on GitHub) and find this line inside the `<script>` tag:

```javascript
// LLM API Key and URL (Key has been inserted)
// **NOTE**: Replace this placeholder key with your actual Gemini API Key for transcription to work.
const apiKey = "AIzaSyBMRBIhCZCBb6K6Muy6BkYax2M1XYCamiw";
