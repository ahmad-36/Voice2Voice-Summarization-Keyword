# Voice-to-Voice Multilingual Translator

## Overview
The **Voice-to-Voice Multilingual Translator** is a Python-based application that transcribes speech from an audio input, translates it into multiple languages (Spanish, Turkish, and Japanese), and converts the translated text back into speech using **ElevenLabs**.

## Features
- **Speech-to-Text:** Uses **AssemblyAI** for transcribing speech from an audio file.
- **Translation:** Utilizes the `translate` module to translate English text into Spanish, Turkish, and Japanese.
- **Text-to-Speech:** Converts translated text into speech using **ElevenLabs API**.
- **User Interface:** Built with **Gradio**, allowing users to interact with the application via a web-based UI.

## Installation
### Prerequisites
Ensure you have Python installed (recommended: Python 3.8 or higher). You also need to install the required dependencies.

### Install Required Libraries
Run the following command to install the necessary dependencies:

```sh
pip install gradio assemblyai translate elevenlabs
```

## Usage
### 1. Clone the Repository
```sh
git clone https://github.com/ahmad-36/Voice2Voice-Summarization-Keyword.git
cd Voice2Voice-Summarization-Keyword
```

### 2. Set Up API Keys
You need API keys for **AssemblyAI** and **ElevenLabs**. Replace the placeholders in the script with your actual API keys:
- **AssemblyAI API Key:** Set in `audio_transcription()` function.
- **ElevenLabs API Key:** Set in `text_to_speech()` function.

### 3. Run the Application
Execute the script with:

```sh
python simple_vtv.py
```

The **Gradio** interface will launch, allowing you to input audio and receive translated voice outputs.

## Project Workflow
1. **User speaks into the microphone.**
2. **Speech is transcribed into text** using AssemblyAI.
3. **Text is translated** into Spanish, Turkish, and Japanese.
4. **Translated text is converted to speech** using ElevenLabs.
5. **Translated audio is played back** to the user via Gradio.

## File Structure
```
Voice2Voice-Summarization-Keyword/
│── simple_vtv.py            # Main script
│── requirements.txt         # List of dependencies
│── README.md                # Project documentation
```

## Dependencies
- **Gradio** – For creating the user interface
- **AssemblyAI** – For speech-to-text conversion
- **Translate** – For text translation
- **ElevenLabs** – For text-to-speech conversion

## Notes
- Ensure you have a stable internet connection for API calls.
- Modify the **voice_id** in `text_to_speech()` to use a different ElevenLabs voice.


---

For contributions or issues, feel free to open a pull request or an issue on [GitHub](https://github.com/ahmad-36/Voice2Voice-Summarization-Keyword).

