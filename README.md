# Video Transcription and Audio Replacement with Grammar Correction

This Python project automates the process of transcribing the audio from a video file, correcting grammatical errors in the transcription, and generating a new audio track using text-to-speech, which is then synced and reassigned to the original video.

## Features

- **Audio Transcription:** Extracts audio from a video and converts it to text.
- **Grammar Correction:** Corrects grammatical mistakes in the transcription using AI.
- **Text-to-Speech Conversion:** Converts the corrected transcription back to audio using a text-to-speech engine.
- **Audio Replacement:** Syncs the new audio with the original video, ensuring accurate timing and alignment.

## Technologies Used

- **Python 3.x**
- **gTTS (Google Text-to-Speech)** for generating audio from corrected text.
- **Azure Chat API** for grammar correction in the transcription.
- **Pydub** for audio processing and manipulation.

## Prerequisites

Ensure you have the following installed on your local machine:

- **Python 3.x**
- **pip** (Python package installer)

### Required Libraries

Install the necessary Python libraries by running:

```bash
pip install -r requirements.txt
