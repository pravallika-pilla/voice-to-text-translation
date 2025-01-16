# voice-to-text-translation
A Python application for voice-to-text translation with language detection and audio output.

Voice-to-Text Translation Application 🎙️🌐
This project is a Python-based application that captures voice input, recognizes the spoken text, detects its language, translates it into a target language, and generates an audio file in the translated language. It's a simple yet powerful demonstration of speech recognition, language translation, and text-to-speech synthesis.

Features ✨
* Voice Input: Captures speech via microphone.
* Speech Recognition: Recognizes spoken text using Google Speech Recognition.
* Language Detection: Automatically detects the language of the recognized text.
* Translation: Translates text into a user-specified target language.
* Audio Output: Converts the translated text into an audio file using Google Text-to-Speech (gTTS).
* Cross-Platform: Works on macOS, Linux, and Windows (with appropriate configurations).

Prerequisites 📋
Ensure the following are installed:
* Python 3.7 or higher
* Microphone access
* Required Python libraries

Supported Languages 🌍
The application currently supports translation to the following languages:
1. Hindi (hi)
2. Telugu (te)
3. Kannada (kn)
4. Tamil (ta)
5. Malayalam (ml)
6. Bengali (bn)

Installation ⚙️
1. Clone this repository:
   git clone https://github.com/<your-username>/voice-to-text-translation.git
   cd voice-to-text-translation
2.Set up a virtual environment (optional but recommended):
   python3 -m venv venv
   source venv/bin/activate  # For macOS/Linux
   venv\Scripts\activate     # For Windows
3.Install dependencies:
   pip install -r requirements.txt
4.Ensure microphone permissions are enabled:
  On macOS: Go to System Preferences > Security & Privacy > Microphone and ensure your terminal app is checked.

Usage 🚀
1. Run the application:python app.py
2. Follow the prompts:
    * Enter the target language (e.g., Hindi, Telugu).
    * Speak into the microphone when prompted.
3.Output:
    * Recognized text is displayed in the terminal.
    * Translated text is displayed.
    * Translated audio is saved in the outputs/ folder and automatically played.
Known Issues 🛠️
* PyAudio Installation on macOS: Ensure portaudio is installed via Homebrew:
  brew install portaudio
  LDFLAGS="-L/usr/local/lib" CFLAGS="-I/usr/local/include" pip install pyaudio  
* Translation Limitations: The googletrans library may occasionally fail due to API limitations. Retry if translation fails.

Future Enhancements 🚀
* Add a GUI for improved user interaction.
* Support for more languages.
* Extend functionality for batch audio file translation.

Acknowledgements 🙌
* Google Speech Recognition
* Google Translate API
* gTTS (Google Text-to-Speech)


