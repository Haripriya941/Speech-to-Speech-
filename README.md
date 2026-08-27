
# Speech Recognition using Python

## 📌 Project Description

This is a simple **Speech Recognition** project developed using Python.

The program listens to the user's voice through the microphone and converts the spoken words into text using the `SpeechRecognition` library and Google's speech recognition service.

## 🛠️ Technologies Used

* Python
* SpeechRecognition
* Microphone
* Google Speech Recognition

## 📂 Project Structure

```text
Speech-Recognition/
│
├── speech_recognition.py
└── README.md
```

## ⚙️ Installation

Install the required library using:

```bash
pip install SpeechRecognition
```

For microphone support, install PyAudio:

```bash
pip install PyAudio
```

## ▶️ How to Run

Run the Python program using:

```bash
python speech_recognition.py
```

The program will display:

```text
Speak Anything :
```

Speak something through your microphone.

The recognized text will be displayed as:

```text
You said : Hello
```

## 💻 Code

```python
import speech_recognition as sr

r = sr.Recognizer()

with sr.Microphone() as source:
    print("Speak Anything :")
    audio = r.listen(source)

try:
    text = r.recognize_google(audio)
    print("You said :", text)

except:
    print("Sorry could not recognize your voice")
```

## ✨ Features

* Takes voice input through a microphone
* Converts speech into text
* Uses Google Speech Recognition
* Simple and beginner-friendly
* Displays the recognized text in the terminal

## ⚠️ Note

An active internet connection may be required for Google Speech Recognition to process the audio.

## 👩‍💻 Author

**Haripriya G.**
