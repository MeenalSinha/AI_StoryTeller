---

# 🎭 Interactive AI StoryTeller

### 🧠 A Creative AI App that Generates, Narrates & Exports Stories from Images

---

## 📌 Overview

**AI StoryTeller** is an interactive project that combines **Computer Vision**, **Natural Language Processing**, and **Text-to-Speech** to create imaginative stories from uploaded images.
It uses **BLIP (Bootstrapped Language Image Pretraining)** for image captioning and **gTTS** for generating spoken narration, allowing users to **see, read, and hear** AI-generated stories.

This notebook/app showcases how AI can be used creatively to **interpret visual input** and **generate contextually meaningful narratives**, exported as both **audio** and **PDF storybooks**.

---

## 🚀 Features

* 🖼 **Image Captioning** with BLIP Transformer
* ✍️ **Story Generation** based on image description
* 🔊 **Text-to-Speech Narration** via Google TTS
* 📄 **Automatic PDF Storybook Creation** (with embedded images)
* 🌐 **Streamlit App Integration** for interactive use
* ⚡ **Ngrok Tunnel Support** for Colab-based deployment

---

## 🛠 Technologies Used

| Category             | Libraries / Tools                                               |
| -------------------- | --------------------------------------------------------------- |
| **Core AI/ML**       | `transformers`, `BLIPProcessor`, `BLIPForConditionalGeneration` |
| **Audio Generation** | `gTTS`                                                          |
| **UI / App**         | `streamlit`, `pyngrok`                                          |
| **PDF Generation**   | `reportlab`                                                     |
| **Image Handling**   | `Pillow (PIL)`                                                  |
| **Environment**      | `Python 3.x`, `Google Colab`                                    |

---

## ⚙ Installation

```bash
# 1️⃣ Clone the repository
git clone https://github.com/MeenalSinha/AI_StoryTeller.git
cd AI_StoryTeller

# 2️⃣ (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate      # On macOS/Linux
venv\Scripts\activate         # On Windows

# 3️⃣ Install dependencies
pip install -r requirements.txt
```

---

## ▶ Usage

### 💡 Option 1: Run in Google Colab

Open the notebook:

```bash
AI_StoryTeller.ipynb
```

Follow the steps:

1. Upload an image
2. Generate a description using BLIP
3. Convert it into a short story
4. Listen to the narration
5. Export as a PDF storybook

---

### 💻 Option 2: Run the Streamlit App

```bash
streamlit run app_streamlit_story.py
```

Then open the public URL provided by **ngrok** to interact with the live app.

---

## 📊 Workflow

1. **Upload Image** → via Streamlit or notebook cell
2. **Generate Caption** → using BLIP model (`Salesforce/blip-image-captioning-base`)
3. **Create Story** → based on AI-generated caption
4. **Narrate Story** → with `gTTS` (Text-to-Speech)
5. **Export PDF** → image + storybook saved locally

---

## 📂 File Structure

```
AI_StoryTeller/
│
├── app_streamlit_story.py      # Streamlit app script
├── AI_StoryTeller.ipynb        # Colab notebook
├── requirements.txt            # Dependencies
├── story_outputs/              # Generated PDFs & audio
└── assets/                     # Sample images
```

---

## 🎧 Example Output

**Input Image:** Uploaded by user
**Generated Story:**

> “As the sun set beyond the mountains, the traveler paused, feeling the warmth fade into whispers of twilight…”

**Audio Output:** Generated MP3 narration
**Exported File:** `Story_Output.pdf`

---

## 👨‍💻 Author

**Meenal Sinha**
📧 [meenal.sinha09@gmail.com](mailto:meenal.sinha09@gmail.com)
🌐 [GitHub – MeenalSinha](https://github.com/MeenalSinha)

---
