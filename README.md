# SoulX-FlashHead: AI Talking Head Generator

SoulX-FlashHead is a real-time, audio-driven talking head generation system. It can animate a portrait image based on any speech input, providing high-quality, synchronized facial movements.

---

Generate video 9:16 -> [![ Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/QasimSalemm/talking/blob/main/SoulX_FlashHead_colab.ipynb)

Generate Image 9:16 -> [![Generate Image Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/QasimSalemm/talking/blob/main/Image_Turbo_colab.ipynb) 

---

## ⚡ Features

- **Lite & Pro Modes**: Choose between high speed (Lite) or high quality (Pro).
- **Real-time Performance**: Optimized for fast generation on modern GPUs (96 FPS on RTX 409).
- **Face Detection Fix**: Custom OpenAI-based face handler to replace broken mediapipe dependencies, ensuring stable inference on Linux/Colab.
- **Aspect Ratio support**: Patched for 16:9 and other resolutions with automated compositing.
- **Easy UI**: Built-in Gradio web interface with public URL sharing.

## 🚀 Getting Started

### Google Colab

The easiest way to run this project is on Google Colab with a free T4 GPU. 
1. Click the **Open In Colab** badge above.
2. In Colab, go to **Runtime** > **Change runtime type** and select **T4 GPU**.
3. Run all cells sequentially.

### Local Installation

For local use, follow these steps:

1. **Environment Setup**:
   ```bash
   conda create -n flashhead python=3.10
   conda activate flashhead
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the App**:
   ```bash
   python gradio_app.py
   ```

## 📥 Model Weights

The models are automatically downloaded in the Colab notebook. For local use, you can download them from Hugging Face:
- [SoulX-FlashHead-1_3B](https://huggingface.co/Soul-AILab/SoulX-FlashHead-1_3B)
- [wav2vec2-base-960h](https://huggingface.co/facebook/wav2vec2-base-960h)