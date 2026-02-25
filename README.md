# 🎬 GENPro — Text-to-Image & Video Generator

A **cinematic, Netflix-style AI generation dashboard** built with Stable Diffusion and Gradio.
Generate high-quality images and short videos from natural language prompts with a professional UI and production-ready pipeline.

---

## ✨ Features

### 🖼️ Image Generation

* Stable Diffusion v1.5 powered
* Prompt enhancement system
* Negative prompt support
* Style presets (Realistic, Anime, Cyberpunk, Fantasy, etc.)
* Seed control for reproducibility
* Resolution control
* Turbo mode for faster generation
* History gallery
* One-click image download

### 🎬 Text-to-Video (Lite)

* Multi-frame diffusion video synthesis
* Cinematic prompt injection
* MP4 export
* Works on Colab GPU

### 🎨 Professional UI

* Netflix-inspired dark dashboard
* Glassmorphism cards
* Hero header
* Two-panel studio layout
* Responsive Gradio interface
* Shareable public link

---

## 🏗️ Tech Stack

* **Python**
* **Diffusers**
* **Stable Diffusion v1.5**
* **PyTorch**
* **Gradio**
* **ImageIO**
* **Google Colab (recommended)**

---

## 🚀 Demo Workflow

```
User Prompt
   ↓
Prompt Enhancement
   ↓
Stable Diffusion Pipeline
   ↓
Image/Video Output
   ↓
Gallery + Download
```

---

## 📦 Installation

### ✅ Recommended: Google Colab

1. Open a new Colab notebook
2. Enable GPU:

   ```
   Runtime → Change runtime type → GPU
   ```
3. Install dependencies:

```bash
pip install diffusers transformers accelerate torch gradio pillow imageio imageio-ffmpeg
```

---

## ▶️ How to Run

### Step 1 — Load the model

The notebook automatically downloads:

* Stable Diffusion v1.5 (~4GB)

First run may take a few minutes.

---

### Step 2 — Launch the UI

```python
demo.launch(share=True)
```

You will get:

* Local URL
* Public Gradio link

---

### Step 3 — Generate

1. Enter prompt
2. Choose style
3. Adjust settings
4. Click **Generate**

---

## 🎛️ Key Controls Explained

| Control         | Purpose                |
| --------------- | ---------------------- |
| Prompt          | Main image description |
| Negative Prompt | What to avoid          |
| Style Preset    | Adds artistic bias     |
| Steps           | Quality vs speed       |
| Guidance Scale  | Prompt strength        |
| Seed            | Reproducibility        |
| Turbo Mode      | Faster generation      |

---

## ⚡ Performance Tips

### 🟢 For Colab T4

* Steps: 20–30
* Resolution: 512×512
* Turbo: ON for speed

### 🔵 For A100

* Steps: 30–40
* Resolution: 768×768
* Turbo: OFF for quality

---

## 📁 Suggested Project Structure

```
ai-studio-pro/
│
├── app.ipynb
├── README.md
├── requirements.txt
└── assets/
```

---

## 🧠 Future Improvements

* [ ] SDXL support
* [ ] AnimateDiff integration
* [ ] ControlNet
* [ ] Inpainting
* [ ] Batch generation
* [ ] Prompt auto-LLM enhancer
* [ ] Hugging Face Spaces deployment
* [ ] User authentication

---

## ⚠️ Limitations

* Video generation is lightweight (not full diffusion video)
* First model load is large (~4GB)
* Best performance requires GPU
* Not trained from scratch (uses pretrained diffusion)

---

## 🙌 Acknowledgements

* Stability AI
* Hugging Face Diffusers
* Gradio Team

---

## 📜 License

This project is for **educational and research purposes**.
Check model licenses before commercial use.

---

## ⭐ If You Like This Project

Give it a star ⭐ on GitHub — it helps a lot!

---

**Built with ❤️ for AI creators and builders**
