# 🎧 Kinyarwanda ASR Qualitative Evaluation

This project performs **qualitative analysis** of an **Automatic Speech Recognition (ASR)** model on the **Kinyarwanda** language using Hugging Face pipelines. It compares transcriptions from the model against ground truth, highlights word-level differences, and displays them in color-coded format for easy human inspection.

## ✅ Features

- Loads audio samples and reference transcripts from a dataset on Hugging Face
- Performs transcription using a pre-trained ASR model (e.g. Whisper, MMS)
- Computes WER and CER for each sample
- Prints color-coded visual diffs between predicted and reference transcriptions:
  - ✅ Matches
  - ❌ Substitutions / Errors
- Saves detailed CSV results per audio sample

## 🔤 Language Focus

- **Language:** Kinyarwanda (`kin`)
- **Dataset:** `KYAGABA/kinyarwanda_cleaned_testset`

## 🧪 Model

Supports any Hugging Face ASR model, example:
```python
model_name = "asr-africa/whisper-small-kinyarwanda_300hrs"
