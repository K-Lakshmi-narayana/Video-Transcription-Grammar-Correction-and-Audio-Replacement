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
```


## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/video-audio-replacement.git
cd video-audio-replacement
```
## Set up API keys:

To use the Azure Chat API for grammar correction, you will need to set up your API keys in the project.
Create a .env file in the root directory with your API keys:

```bash
AZURE_API_KEY=your_azure_api_key
AZURE_ENDPOINT=your_azure_endpoint
```
### Usage
Place your video file in the input/ directory (or modify the path in the script accordingly).

Run the script to process the video file:

```bash
python process_video.py --input input/video.mp4 --output output/final_video.mp4
```
This will:

- Extract the audio from the video.
- Transcribe the audio and correct any grammatical mistakes.
- Generate a new audio file with corrected speech.
- Sync and replace the original audio in the video.

The final video with the corrected audio will be saved in the output/ directory.

### Example Workflow

- Extract audio from the input video.
- Transcribe audio using Azure Chat API.
- Correct grammatical errors in the transcription.
- Convert the corrected text into audio using gTTS.
- Replace the original audio with the new, grammatically correct audio in the video file.

## Configuration
You can configure the following options in the config.json file:

- **silence_timing:** Adjust how long the silences between sentences should last, based on original timestamps.
- **voice_language:** Specify the language for text-to-speech conversion (default is en for English).

## Known Issues

- **Audio Syncing:** In some cases, slight misalignment may occur if the original transcription has significant timing issues. This can be adjusted by modifying the silence duration in the script.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue if you find a bug or have suggestions for new features.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
For any questions or feedback, feel free to reach out to me at klaxminarayana2004@gmail.com
