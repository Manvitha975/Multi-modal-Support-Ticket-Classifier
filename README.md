# 🎧 Multi-modal Support Ticket Classifier

An intelligent support ticket classification system that uses **text, image, and optional audio inputs** to automatically categorize incoming support tickets.

---

## 🚀 Features

- 📝 **Text Processing (BERT)**  
  Uses `bert-base-uncased` to extract meaningful text embeddings.

- 🖼️ **Image Feature Extraction (ResNet18)**  
  Processes uploaded screenshots or images.

- 🎙️ **Audio Transcription (Whisper)**  
  Converts voice messages into text for classification.

- 🔗 **Multi-modal Fusion Model**  
  Combines text + image + audio features for accurate prediction.

- 📊 **Confidence Scores & Logging**  
  Displays prediction probabilities and logs results.

---

## 🧠 Model Architecture

- **Text** → BERT → 256-dim projection  
- **Image** → ResNet18 → 256-dim projection  
- **Fusion** → Concatenation → Linear (512 → 128) → Dropout → Final Classifier  

---

## 📁 Project Structure

``` id="f9j2lm"
📁 multi-modal-support-classifier
│-- App.py
│-- train.py
│-- process.py
│-- multimodal_classifier.pth
│-- label_classes.csv
│-- all_tickets_processed_improved_v3.csv
│-- prediction_logs.csv
│-- dataset/
│-- README.md
