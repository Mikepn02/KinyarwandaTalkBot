# KinyarwandaTalkBot 🤖


## Installation 💻

### Prerequisites
- Python 3.12
- FFmpeg (audio processing):
  ```bash
  # Ubuntu/Debian
  sudo apt-get install ffmpeg
  
  # macOS
  brew install ffmpeg
  
  # Windows (via chocolatey)
  choco install ffmpeg
  ```
  
## Quick Start 🚀

- Clone repository
  ```bash
    git clone https://github.com/mikepn02/KinyarwandaTalkBot.git
    cd KinyarwandaVoiceAssistant
  ```
- Set up virtual environment
  ```bash
  python -m venv .venv
  source .venv/bin/activate  # Linux/macOS
  .\.venv\Scripts\activate   # Windows

  ```
- Install dependencies
  ```bash
  pip install -r requirements.txt
  ```

## Configuration ⚙️

#### QA Configuration in `nlp_mapping.json`

  ```json
  {
    "qa_pairs": [
      {
        "question": "Mwaramuce neza?",
        "answer": "Mwaramutse! Amakuru yanyu?"
      }
    ],
    "default_response": "Vugurura ikibazo."
  }
  ```

#### Audio Files
You can find sample Kinyarwanda recordings in the `/sample_inputs` folder

Supported formats: `WAV`, `MP3`, `OGG`


## Usage 🚀

#### Start the application
  ```bash
  python main.py
  ```

#### Access the interface
- Navigate to http://localhost:7860

## Interface Guide 💡
1. Record using your microphone or upload an audio file
1. Click **Submit** to process (⏳ ~10–60 sec)
1. Response audio auto-plays
1. Review **Conversation History**:
   - Raw transcription
   - Matched question key
   - Generated response
1. Click **Clear** to reset session

## Example Interactions 🗣️
| Raw Transcription | Matched Question | System Response                                              |
|-------------------|-----------|--------------------------------------------------------------|
| mizeneza          |Umeze neza?| Yego! Turashima Imana.                                       |
| wakorewee heheh   |Wakorewe hehe?| Nakorewe muri Rwanda Coding Academy, nakozwe na Mike Nzabera. |