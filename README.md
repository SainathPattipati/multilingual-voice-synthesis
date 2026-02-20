# Multilingual Voice Synthesis

Text-to-speech pipeline supporting 20+ languages with voice cloning and emotion control.

## Features

- Multi-language support (20+)
- Voice cloning from reference audio
- Emotion control (happy, sad, neutral, etc.)
- Audio post-processing
- Format conversion

## Supported Languages

English, Spanish, French, German, Mandarin, Japanese, Hindi, Korean, Portuguese, 
Russian, Italian, Dutch, Polish, Turkish, Swedish, Danish, Norwegian, Finnish, 
Czech, Hungarian, and more.

## Installation

```bash
pip install -r requirements.txt
```

## Quick Start

```python
from src.synthesis.tts_pipeline import TTSPipeline

pipeline = TTSPipeline()
audio = pipeline.synthesize(
    text="Hello, world!",
    language="en",
    emotion="happy"
)
```

## Dependencies

- elevenlabs >= 0.2.0
- langdetect >= 1.0.9
- pydub >= 0.25.0
- numpy >= 1.21.0
- pydantic >= 1.10.0

## License

MIT License
