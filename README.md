# Speech Emotion Recognition and Gender Detection Application

## Overview
This project is a Flask-based application that performs the following features:
- **Emotion Recognition**: Detects emotions from speech inputs.
- **Gender Detection**: Classifies the speaker’s gender as male or not male.
- **Speech-to-Text**: Converts speech input into text.
- **Sentiment Analysis**: Analyzes the sentiment of the transcribed text.

The application leverages state-of-the-art transformer models and advanced preprocessing techniques to deliver accurate results, aiming to serve a wide range of users.

---

## Features
1. **Emotion Recognition**
   - Identifies emotions such as happiness, sadness, anger, surprise, and more.
   - Model used: `r-f/wav2vec-english-speech-emotion-recognition`.

2. **Gender Detection**
   - Classifies the speaker’s gender.
   - Model used: `alefiury/wav2vec2-large-xlsr-53-gender-recognition-librispeech`.

3. **Speech-to-Text**
   - Converts speech input to text for further analysis.
   - Utilizes libraries like SpeechBrain and Librosa.

4. **Sentiment Analysis**
   - Analyzes the sentiment (positive, neutral, or negative) from the transcribed text.
   - Powered by Hugging Face transformers.

---

## Tech Stack
- **Frameworks**: Flask, SpeechBrain
- **Libraries**:
  - `torchaudio`, `librosa` for audio processing
  - `transformers` for model integration
  - `pyngrok` for endpoint tunneling
  - `huggingface_hub` for accessing pre-trained models
  - `pandas`, `numpy` for data handling
- **Models**:
  - Emotion Detection: `r-f/wav2vec-english-speech-emotion-recognition`
  - Gender Detection: `alefiury/wav2vec2-large-xlsr-53-gender-recognition-librispeech`
- **Environment**: Google Colab (for running and testing)

---

## Installation
### Prerequisites
- Python 3.8+
- Pip (Python package manager)
- Ngrok account (for exposing local Flask app)

### Steps
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Flask application:
   ```bash
   python app.py
   ```

4. Use ngrok to expose your local server:
   ```bash
   ngrok http 5000
   ```

5. Access the application using the provided ngrok URL.

---

## Usage
1. **Upload an audio file** in WAV format.
2. The application will process the audio and display:
   - Detected emotion
   - Speaker’s gender
   - Transcribed text
   - Sentiment analysis of the text

---

## Folder Structure
```plaintext
.
├── app.py              # Main Flask application
├── models/             # Pre-trained models and checkpoints
├── static/             # Static files (CSS, JavaScript)
├── templates/          # HTML templates for Flask app
├── requirements.txt    # Dependencies
├── README.md           # Project documentation
└── utils.py            # Utility functions for preprocessing and inference
```

---

## Examples
### Input
An audio file (e.g., `speech_sample.wav`).

### Output
- **Emotion**: Happy
- **Gender**: Male
- **Transcribed Text**: "I am feeling great today."
- **Sentiment**: Positive

---

## Models
### Emotion Detection
- **Model**: `r-f/wav2vec-english-speech-emotion-recognition`
- **Framework**: Hugging Face Transformers

### Gender Detection
- **Model**: `alefiury/wav2vec2-large-xlsr-53-gender-recognition-librispeech`
- **Framework**: Hugging Face Transformers

---

## Future Enhancements
1. Integrate support for real-time audio input via microphone.
2. Add more emotions and languages.
3. Optimize for large-scale deployment to support over 1 lakh users.

---

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Added a new feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact
For any questions or feedback, feel free to reach out to me:
- **Name**: Sankalp Dwivedi
- **Email**: [dwivedisankalp02@gmail.com]
- **LinkedIn**: [sankalp-dwivedi-9b18b320b](https://www.linkedin.com/in/sankalp-dwivedi-9b18b320b/)

