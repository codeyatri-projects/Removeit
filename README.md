# 🧹 Remove-It — AI Background Remover


![WhatsApp Image 2025-10-22 at 19 11 40_7aff9761](https://github.com/user-attachments/assets/8e310aaa-f143-4473-b320-417dfe8c5198)

### ✨ Remove backgrounds instantly using AI (U²Net model)  
Fast, lightweight, and production-ready — powered by **FastAPI**, **rembg**, and **Render**.

---

🔗 **Use it here:** [https://removeit.codeyatri.space](https://removeit.codeyatri.space)
---



## 🚀 Features

- ⚡ **Instant AI background removal** using the **U²Net** model from `rembg`.
- 🧠 **Fully API-based backend** built with **FastAPI**.
- 🧩 **Automatic cache cleanup** using socket-based file management.
- 🪶 **Lightweight & Render-optimized** — prevents storage overflows.
- 💾 **Large model handling** through **Git LFS**.
- 🌍 **Deployed on Render** with seamless CI/CD from GitHub.

---

## 🧠 Tech Stack

| Layer | Technology |
|:------|:------------|
| Backend | 🐍 FastAPI |
| AI Model | 🧠 rembg (U²Net) |
| Image Processing | 🖼️ Pillow |
| Deployment | 🚀 Render |
| Storage | 📦 Git LFS |
| Cleanup | 🔌 Custom socket-based file cleaner |

---


🧼 Smart Cache Cleaning System

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


Developed by Codeyatri

“A clean image deserves a clean background.”
