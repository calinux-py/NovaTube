# NovaTube - YouTube Analyzer

NovaTube is a desktop application that allows you to analyze YouTube videos by downloading their audio, transcribing the content, and generating AI-powered analysis using ChatGPT. The application features a modern, dark-themed UI built with PyQt5 and provides an intuitive way to process YouTube content.

## Features

- Download audio from YouTube videos
- Automatic speech-to-text transcription using Whisper AI
- AI-powered content analysis using ChatGPT
- Custom analysis instructions configuration
- Progress tracking for each processing step
- HTML report generation with copy functionality
- Configurable OpenAI API settings

## Requirements

- Python 3.7+
- PyQt5
- yt-dlp
- OpenAI Whisper
- OpenAI API access

## Installation

1. Clone the repository or download the source code
2. Install the required dependencies:

```bash
pip install PyQt5 yt-dlp openai-whisper openai
```

## Configuration

Before using the application, you need to:

1. Obtain an OpenAI API key from [OpenAI's website](https://openai.com)
2. Enter your API key in the Settings tab of the application
3. Customize the AI analysis instructions in the Settings tab

## Usage

1. Launch the application:
```bash
python novatube.py
```

2. Enter a YouTube URL in the main interface
3. Click "Analyze" to start the process
4. Monitor the progress through the status updates and progress bar
5. Once complete, a HTML report will automatically open in your default browser

## Report Format

The generated report includes:
- Video title
- Complete transcript divided into paragraphs
- AI analysis based on your custom instructions
- Copy functionality for both transcript and analysis
- Dark-themed interface for better readability

## Directory Structure

```
novatube/
├── config/
│   ├── config.ini    # API key configuration
│   └── prompt.ini    # Custom AI instructions
├── downloads/        # Temporary audio files
└── report.html      # Generated analysis report
```
