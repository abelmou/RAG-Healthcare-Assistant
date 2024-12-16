# RAG-Powered Healthcare Assistant

An AI-driven healthcare assistant that utilizes Retrieval-Augmented Generation (RAG) with multilingual support in Darija, Arabic, and English to offer personalized health management. The app helps users with prescription scanning, health queries, multilingual support, and pharmacy locator.

- Watch the video demo of our app [video-demo](https://shorturl.at/HHoY6).

## Background and Problem Statement

Managing healthcare information effectively remains a challenge in today's world. Common issues include:

- Fragmented medical records
- Difficulty in obtaining personalized medical advice
- Language barriers in healthcare communication
- Difficulty locating nearby healthcare providers

## Impact and Proposed Solution

The **RAG-Powered Healthcare Assistant** aims to solve these challenges by:

- Centralizing personal health records for easy access
- Leveraging RAG to provide intelligent, context-aware responses to health queries
- Enabling Prescription OCR for easy scanning and processing of prescriptions
- Offering multilingual support (Darija, Arabic, English) for diverse users
- Incorporating a Pharmacy Locator with geolocation to help users find nearby pharmacies and healthcare providers

## Project Outcomes and Deliverables

This project delivers:

- A fully functional AI-powered healthcare assistant
- A multilingual chatbot for health queries
- An OCR system for prescription scanning and processing
- An integrated Pharmacy Locator with real-time geolocation
- Secure storage and retrieval of personalized medical records

## Technology Stack

- **Frontend**: 
  - Streamlit - Main web interface
  - Chainlit - Chat interface
- **Backend**:
  - Python 3.9+
  - LangChain - For AI/LLM orchestration
  - ChromaDB - Vector database for document storage
  - Ollama - Local LLM integration
  - OpenCV - Image processing
  - PyPDF & PDFPlumber - PDF processing
  - Unstructured - Document parsing
  - ElevenLabs - Text-to-speech capabilities

## Prerequisites

Before running the application, ensure you have:

1. Python 3.9 or higher installed
2. Git installed
3. Ollama installed (for local LLM support)
4. Sufficient disk space for dependencies and document storage
5. A modern web browser

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/abelmou/RAG-Healthcare-Assistant.git
   cd RAG-Healthcare-Assistant
   ```

2. Create and activate a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Install and start Ollama (if not already done):
   ```bash
   # Follow Ollama installation instructions at: https://ollama.ai/
   # Pull the required model:
   ollama pull llama3.2
   ```

## Installation and Setup

1. OCR Interface (for prescription scanning):
   ```bash
   streamlit run ocr.py
   ```

2. Pharmacy Locator Interface:
   ```bash
   streamlit run pharmascysol.py
   ```

3. Chainlit Chat Interface (for health queries):
   ```bash
   chainlit run app_chainlit.py
   ```

4. Streamlit Main Interface:
   ```bash
   streamlit run app_streamlit.py
   ```

The application will be accessible through your web browser at the provided local URL.

## Future Enhancements
- Expanding language support to more regions and dialects.
- Improving OCR accuracy and expanding prescription types supported.
- Adding integration with healthcare provider APIs for real-time health data.