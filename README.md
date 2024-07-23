# YouTube Chapter Generator

This project provides a tool for transcribing audio from YouTube videos and generating YouTube chapters using Cohere's language models. The tool supports transcription using either Whisper or AssemblyAI and adds timestamps every minute for easy segmentation.

## Features

- Download audio from YouTube videos
- Transcribe audio using Whisper or AssemblyAI
- Generate YouTube chapters using Cohere's language models
- Save transcriptions and chapters to text files

## Getting Started

### Prerequisites

- Python 3.8 or higher
- [Whisper](https://github.com/openai/whisper) (optional, for Whisper transcription)
- [AssemblyAI](https://www.assemblyai.com) (optional, for AssemblyAI transcription)
- [Cohere](https://cohere.ai)
- [FFmpeg](https://ffmpeg.org) (required for Whisper)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/gmbabreu/YouTube-Chapter-Generator.git
    cd YouTube-Chapter-Generator
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. Install FFmpeg (for Whisper transcription):
    - **Windows**: Download and install FFmpeg from [FFmpeg Windows](https://ffmpeg.org/download.html#build-windows).
    - **Mac**: Use Homebrew to install FFmpeg:
      ```sh
      brew install ffmpeg
      ```
    - **Linux**: Use your package manager to install FFmpeg. For example, on Ubuntu:
      ```sh
      sudo apt update
      sudo apt install ffmpeg
      ```

4. Set up environment variables:
    Create a `.env` file in the root directory and add your API keys:
    ```
    COHERE_API_KEY=your_cohere_api_key
    ASSEMBLYAI_API_KEY=your_assemblyai_api_key
    ```

### Usage

#### Transcription with Whisper

1. Choose your transcribing method. To use AssemblyAI you must gain access to their API keys 
2. Configure the audio_path variable to the path for your audio file.
3. Run one of the scripts:
    ```sh
    python chapter_generator_whisper.py
    ```

