# 🤖 Voice2Sign: Speech-to-Indian Sign Language Translator

This project captures spoken English using a microphone, processes it using audio signal processing and speech recognition, and maps the result to **Indian Sign Language (ISL)** using pre-saved GIFs or alphabet images. It is a great assistive tool for translating voice into visual ISL representations.

---

## 🎯 Features

- 🎙️ Real-time voice recording (using microphone)
- 🎧 Audio feature extraction with mel-spectrograms and MFCC
- 🧠 Converts speech to text using Google Speech Recognition
- 🧩 Matches recognized phrases with pre-existing ISL GIFs
- 🔤 Falls back to showing alphabet images if full phrase isn't available
- 🖼️ GUI with `easygui` and `tkinter` for a simple interactive experience

---

## 🧱 Architecture

```
+------------------+      +---------------------+      +-----------------+      +-----------------+
| 🎙️ Microphone    | -->  | 🎧 Audio Processing | -->  | 🧠 Speech-to-Text| -->  | ✋ ISL Mapping   |
+------------------+      +---------------------+      +-----------------+      +-----------------+
      User Input             Mel Spectrogram / MFCC        Google API             Show GIF or letters
```

---

## 📁 Folder Structure

```
Voice2Sign/
├── Speech to Indian.ipynb       # Main notebook
├── ISL_Gifs/                    # Folder containing GIFs for predefined ISL phrases
├── letters/                     # Folder containing images for A-Z letters
├── signlang.png                 # Image for easygui popup
├── recording8.wav               # Captured audio file
├── sound9.wav                   # Reconstructed audio after processing
├── README.md                    # Project documentation
└── requirements.txt             # Required packages
```

---

## ⚙️ Installation

1. **Clone the Repository**
```bash
git clone https://github.com/your-username/voice2sign.git
cd voice2sign
```

2. **Install Required Packages**
```bash
pip install -r requirements.txt
```

---

## 📦 Requirements

```
numpy
matplotlib
opencv-python
Pillow
easygui
tk
librosa
soundfile
sounddevice
scipy
wavio
speechrecognition
pyttsx3
pydub
playsound==1.2.2
```

---

## 🚀 How to Run

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `Speech to Indian.ipynb`.

3. Speak when prompted → text is generated → mapped to ISL GIFs or letters.

---

## 📷 Example Output

- If you say: `"good morning"` → it will show `ISL_Gifs/good morning.gif`
- If phrase not found: `"goa"` → it will show letters: `g`, `o`, `a` using images in `/letters/`

---

## 📌 Notes

- Make sure the folders `ISL_Gifs/` and `letters/` exist and contain correct GIF/JPG files.
- Run the notebook in a GUI-capable environment (not headless server) since it uses `tkinter`.

---

## 📜 License

MIT License — free to use and distribute.

---

## 🙌 Acknowledgments

- Google Speech Recognition API
- Librosa for audio analysis
- Indian Sign Language GIF dataset (manually curated)
