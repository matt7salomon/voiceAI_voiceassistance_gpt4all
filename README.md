
# VoiceAI with GPT4All

## Colab notebook
This notebook on google colab has all you need for the voice assistant. The LLM and datasets are on accessible on my shared google drive folder and the notebook should run:
https://colab.research.google.com/drive/1ya9otmKAiqBZViQgUaRJKz-22W2sA81A

## Project description
This project showcases a **voice-controlled AI assistant** using **GPT4All** for conversational AI and speech-to-text capabilities. It listens for a wake word and then processes spoken input using **speech recognition**, generates a response via GPT, and outputs the response through text-to-speech.

## Features

- **Voice Activation**: The AI assistant listens for a user-defined wake word.
- **Speech Recognition**: Converts user speech into text using `speech_recognition`.
- **GPT4All Integration**: Generates natural language responses based on user queries.
- **Text-to-Speech**: The responses are read out loud using `pyttsx3`.

## Installation

To run this notebook, you need to have the following libraries installed. You can install them using pip:

```bash
pip install gpt4all
pip install speechrecognition
pip install pyttsx3
pip install pyaudio
```

Additionally, you may need to install `PyAudio` for handling audio input/output, which can be installed using the following:

```bash
# For Windows
pip install pipwin
pipwin install pyaudio

# For macOS/Linux
brew install portaudio
pip install pyaudio
```

## Usage

1. **Set Wake Word**: The assistant listens for a wake word. Modify the wake word in the code to your preferred word (default: `"GPT"`).
2. **Start the Assistant**: Run the notebook, and the assistant will start listening for the wake word. Once detected, it will prompt the user to speak their query.
3. **Process and Respond**: The assistant will transcribe the user's query, generate a response using GPT4All, and then use text-to-speech to read the response aloud.

### Key Sections

1. **Speech Recognition**:
   - The notebook uses `speech_recognition` to capture and transcribe the user's voice.

2. **GPT4All Integration**:
   - After receiving the user's input, the model generates a response using GPT4All.

3. **Text-to-Speech**:
   - The response is converted into speech and spoken aloud by the assistant.

4. **Continuous Listening**:
   - The assistant continuously listens for the wake word and responds whenever it is triggered.

## Example

Once the assistant is started, it will display:
```
Say GPT to wake me up.
```

Once activated, the assistant will prompt for input:
```
User: [Your spoken prompt]
GPT4All: [Generated response]
```

The response will also be spoken aloud using text-to-speech.

## Requirements

- **Python 3.10+**
- Libraries: `gpt4all`, `speech_recognition`, `pyttsx3`, `pyaudio`

## Notes

- Ensure your microphone is configured correctly, as it is necessary for voice input.
- You can modify the wake word and other parameters (such as maximum tokens for GPT4All) within the notebook.

## License

This project is open-source and free to use under the MIT License.

---


