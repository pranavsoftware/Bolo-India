# 🎙️ Speech to Indian Language Translator

This project is a voice-based translation system that converts spoken English into translated Indian languages like Hindi, Bengali, Tamil, etc. It uses speech recognition, language translation, and text-to-speech to provide both text and audio output in the target language.

---

## ✅ Features

- 🎤 Converts English speech to text
- 🌐 Translates to major Indian languages
- 🔊 Speaks the translated text aloud
- 📔 Easy to run with a single Jupyter notebook

---

## 🧠 Architecture Overview

Here’s a high-level view of how the system works:

```
+------------------+       +----------------------+       +------------------+       +----------------+
|  🎤 User Speaks  | --->  | 🧠 Speech Recognizer | --->  | 🌐 Translator     | --->  | 🔊 Text-to-Speech |
+------------------+       +----------------------+       +------------------+       +----------------+
        Input                  Converts speech                Translates text             Speaks in
     (English audio)             to English text               to Indian lang           Indian language
```

---

## 📁 Folder Structure

```
Speech-to-Indian/
│
├── Speech to Indian.ipynb       # Main Jupyter Notebook
├── README.md                    # This file
├── requirements.txt             # Required Python packages
└── assets/                      # (Optional) Screenshots, audio samples
```

---

## ⚙️ Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/speech-to-indian.git
   cd speech-to-indian
   ```

2. **(Optional) Create a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 How to Run

1. Start Jupyter:
   ```bash
   jupyter notebook
   ```

2. Open `Speech to Indian.ipynb` and run each cell step-by-step.

3. Follow prompts to speak, translate, and hear the output.

---

## 📦 Dependencies

Put this in `requirements.txt`:

```
speechrecognition
googletrans==4.0.0rc1
gTTS
playsound==1.2.2
pyaudio
```

> ⚠️ Note: `pyaudio` might require special installation for your OS.

---

## 🌍 Supported Indian Languages

- Hindi
- Bengali
- Tamil
- Telugu
- Kannada
- Gujarati
- Marathi

---

## 💻 Example Usage

1. You say: “Hello, how are you?”
2. Select target language: Hindi
3. Output: “नमस्ते, आप कैसे हैं?” (text + audio)

---

## 📝 License

MIT License. See [LICENSE](LICENSE) for more info.

---

## 🙌 Acknowledgments

- Google Speech Recognition
- Google Translate API
- gTTS (Google Text-to-Speech)
