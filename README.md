# AI_presenter
Kurdish Sorani AI tv presenter 

# Sorani AI TV Presenter 🎤📺

This project builds a realistic **Kurdish Sorani-speaking AI TV presenter** that can deliver daily 1-minute tech and AI news updates. 
It uses [Coqui TTS](https://github.com/coqui-ai/TTS) for training a custom text-to-speech (TTS) voice and integrates tools to generate videos with lifelike avatars.

---

## 🎯 Goals

- Train a high-quality **Kurdish Sorani voice model**
- Use that voice to generate daily news audio
- Sync audio with a **digital presenter avatar**
- Enable basic AI interaction for co-presenting with a human anchor

---

## 📁 Project Structure


---

## 🧪 How to Train (Quick Start)

1. Prepare your dataset:
   - 1–5 hours of clean Kurdish Sorani speech
   - One sentence per 5–10 sec audio clip
   - Transcripts saved in `metadata.csv` like:
     ```
     0001|ئەمشەو لە هۆشیاری AI باز لە چاتجیپی دەکەین.
     ```

2. Use the Colab notebook `Kurdish_sorani_TTS.ipynb` to train your voice model with Coqui TTS.

3. Generate audio using your trained model:
   ```bash
   tts --text "سڵاو، ئەم ڕاپۆرتەی AI ـیە." --model_path ./your_model.pth

   🧠 Technologies Used (to be confirmed)
Coqui TTS – Text-to-speech engine

Google Colab – Free cloud training

Audacity – Manual audio slicing

OpenAI Whisper – Transcription (optional)

D-ID or HeyGen – Avatar generation

---

## 🧾 `requirements.txt`

```txt
TTS==0.22.0
sox
pydub
whisper
torch>=1.10
torchaudio
transformers>=4.30.0
numpy
scipy
