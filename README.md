<div align="center">

# 👁️ AI Vision Assistant — Real-Time Image Chatbot with TTS

### A Modern Desktop Application that combines Live Camera Vision + AI Chatbot + Text-to-Speech for Accessible Real-Time Understanding.

![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![PyQt5](https://img.shields.io/badge/PyQt5-GUI-41CD52?style=for-the-badge&logo=qt&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Transformers](https://img.shields.io/badge/Transformers-HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)

</div>

---

## 📖 Overview

**AI Vision Assistant** is a modern desktop application designed to help users understand their surroundings using a **real-time camera feed**, an **AI vision-language model**, and **text-to-speech output**.

The system captures an image from the live camera, generates an intelligent response (caption + explanation), and converts it into audio output, enabling fast and accessible interaction for:

- Visually impaired users
- Senior citizens
- Users with low vision
- Users with reading difficulties (e.g., dyslexia)

---

## 🚀 Key Features

### 📷 1. Real-Time Camera Analysis
- Captures images directly from a live camera feed
- Supports real-world environments and dynamic scenes

### 💬 2. Natural Language Interaction
- Users can ask questions like:
  - “What objects do you see?”
  - “Describe this scene.”
  - “What is written here?”
- AI generates a human-friendly response

### 🔊 3. Text-to-Speech (TTS) Responses
- Converts the AI answer into speech output
- Enables hands-free accessibility and faster understanding

### 🖥️ 4. Modern Desktop UI (Dark Theme)
- Clean, responsive PyQt interface
- User-friendly design for non-technical users

### ⚡ 5. Non-Blocking Multi-Threaded Architecture
- Camera runs in its own thread
- AI inference runs in a separate worker thread
- Prevents UI freezing during heavy processing

---

## 🧰 Tech Stack

| Layer | Technology |
|------|------------|
| UI | PyQt5 |
| Computer Vision | OpenCV |
| AI Model | LLaVA (Vision-Language Model) |
| Deep Learning | PyTorch |
| NLP Framework | Transformers |
| Speech | Text-to-Speech (TTS Engine) |

---

## 🏗️ System Architecture

The workflow follows a real-time pipeline:

1. **Start**
2. **Capture Image**
3. **Preprocess Image**
4. **LLaVA Model Processing**
5. **Generate Text**
6. **Generate Audio with TTS**
7. **Provide Output to User**
8. **User Feedback Loop (Refine if needed)**

---

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8+
- Webcam / Camera Device
- (Optional) CUDA GPU for faster inference

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/ai-vision-assistant.git
cd ai-vision-assistant
```
### 2. Install dependencies:
```bash
pip install -r requirements.txt
```

### 3. Download the tiny-llava model:
```bash
git clone https://huggingface.co/bczhou/tiny-llava-v1-hf
```

### 4. Run the application:
```bash
python vision_assistant.py
```
### 👥 Contributors 
- **Ishan Srivastav** – *Testing & Documentation* (System Validation, Report Writing)
- **Priyanshu Kumar Singh** – *Frontend & UI/UX* (PyQt Design, User Experience)
- **Aditya Jaswal** – *Backend & AI Integration* (Model Implementation, System Architecture)

### License

This project is licensed under the MIT License - see the LICENSE file for details.

### Acknowledgments

- [Tiny-LLaVA Model](https://huggingface.co/bczhou/tiny-llava-v1-hf) for image understanding capabilities
- [PyQt5](https://www.riverbankcomputing.com/software/pyqt/) for the UI framework
- [Transformers](https://huggingface.co/docs/transformers/index) by Hugging Face
