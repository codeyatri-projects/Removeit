#  Remove-It — AI Background Remover


![WhatsApp Image 2025-10-22 at 19 11 40_7aff9761](https://github.com/user-attachments/assets/8e310aaa-f143-4473-b320-417dfe8c5198)

###  Remove backgrounds instantly using AI (U²Net model)  
Fast, lightweight, and production-ready — powered by **FastAPI**, **rembg**, and **Render**.

---

🔗 **Use it here:** [https://removeit.codeyatri.space](https://removeit.codeyatri.space)
---

##  The Problem 💡

Designers and editors face one of the most repetitive tasks in their workflow — removing backgrounds. Most available tools either charge for every image or compress the quality. For creative teams working daily with assets, that becomes not only costly but frustrating.

That’s exactly the problem we faced within our own design team — spending hours separating humans from backgrounds. So instead of paying endlessly, we decided to build our own solution.

---

## The Solution

Remove-It is a smart, AI-powered human segmentation and background remover built using U²Net — a state-of-the-art deep learning model for object and human segmentation.

With Remove-It, you can upload an image, and the system automatically detects and isolates human subjects — giving you a clean, transparent background in seconds.

---

##  Features

- ⚡ **Instant AI background removal** using the **U²Net** model from `rembg`.
- 🧠 **Fully API-based backend** built with **FastAPI**.
- 🧩 **Automatic cache cleanup** using socket-based file management.
- 🪶 **Lightweight & Render-optimized** — prevents storage overflows.
- 💾 **Large model handling** through **Git LFS**.
- 🌍 **Deployed on Render** with seamless CI/CD from GitHub.

---

##  Tech Stack

| Layer | Technology |
|:------|:------------|
| Backend | 🐍 FastAPI |
| AI Model | 🧠 rembg (U²Net) |
| Image Processing | 🖼️ Pillow |
| Deployment | 🚀 Render |
| Storage | 📦 Git LFS |
| Cleanup | 🔌 Custom socket-based file cleaner |

---


 Smart Cache Cleaning System

Render’s free tier often crashes due to excess temporary file storage.
To solve this, Remove-It includes a background socket-based cleanup service that:

Automatically detects when cached files exceed safe limits

Removes them without affecting active requests

Keeps disk usage under Render’s quota

This ensures 24/7 uptime and stable memory performance 🧠⚙️

# Clone the repository
git clone https://github.com/yourusername/remove-it.git
cd remove-it

# Install dependencies
pip install -r requirements.txt

# Run the app
uvicorn main:app --host 0.0.0.0 --port 8000

---

## Team CodeYatri
A community for students, designers, and developers to learn, build, and ship real projects together.

👉 Visit www.codeyatri.space

📩 For feedback, collaborations, or improvements: hello@codeyatri.space

“A clean image deserves a clean background.”
