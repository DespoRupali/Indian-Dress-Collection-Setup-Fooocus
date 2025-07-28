# Fooocus + Indian Dress Collection Setup

This README helps you set up and run the **Fooocus** image generation tool with the **Indian Dress Collection By Stable Yogi** model. Ideal for generating high-quality, photorealistic images of Indian traditional dresses.

---

## 📦 Requirements

- Python environment (Colab, Jupyter, or local)
- Stable internet connection
- Recommended: System with high VRAM (Colab Pro or equivalent)

---

## 🛠️ Setup Instructions

1. First, install the required Python package `pygit2`.
2. Clone the official **Fooocus** GitHub repository.
3. Move into the Fooocus directory.
4. Download the custom model titled **Indian Dress Collection By Stable Yogi** from Civitai and place it into the `models/checkpoints/` folder.
5. Launch Fooocus with high VRAM enabled and sharing support.

---

## 🔍 About the Model

- **Name:** Indian_Dress_Collection_By_Stable_Yogi
- **Format:** `.safetensors`
- **Source:** [Civitai - Indian Dress Collection](https://civitai.com/models/324581/indiandresscollectionbystableyogi)
- **Use:** Photorealistic generation of Indian ethnic clothing styles for females

---

## 💻 Commands to Run

```bash
# Step 1: Install required packages
!pip install pygit2==1.15.1

# Step 2: Clone Fooocus repo
%cd /content
!git clone https://github.com/lllyasviel/Fooocus.git
%cd /content/Fooocus

# Step 3: Download the "Indian Dress Collection By Stable Yogi" model
!wget -O /content/Fooocus/models/checkpoints/Indian_Dress_Collection_By_Stable_Yogi.safetensors https://civitai.com/models/324581/indiandresscollectionbystableyogi

# Step 4: Launch Fooocus
!python entry_with_update.py --share --always-high-vram
