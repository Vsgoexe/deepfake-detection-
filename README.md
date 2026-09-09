
# 🚀 Deepfake Detection Project

This project consists of a **FastAPI backend** (Python) and a **React frontend** (Create React App with TailwindCSS).  
Follow the steps below to install and run it locally.

---

## ✅ Prerequisites

Make sure you have these installed on your system before running the project:

- **Python 3.9+** → [Download](https://www.python.org/downloads/)
- **Node.js 18+ (LTS recommended)** → [Download](https://nodejs.org/)
- **npm** (comes with Node.js)
- **Git** (optional, for version control)

Verify installations:
```bash
python --version
node -v
npm -v
git --version
```

---

## ⚡ Backend Setup (FastAPI – Python)

1. Go to the backend folder:
   ```bash
   cd backend-folder
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate    # Windows
   source venv/bin/activate   # Mac/Linux
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the backend server:
   ```bash
   uvicorn main:app --reload
   ```

👉 Backend runs at: **http://127.0.0.1:8000**

⚠️ Required files:
- `models/deepfake_model.h5` (pre-trained deepfake detection model)

---

## 🎨 Frontend Setup (React + Tailwind)

1. Go to the frontend folder:
   ```bash
   cd frontend-folder
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the frontend app:
   ```bash
   npm start
   ```

👉 Frontend runs at: **http://localhost:3000**

---

## 🔄 Running Both Together

- Open **two terminals** (or split terminal):
  - **Terminal 1 → Backend**
    ```bash
    cd backend-folder
    venv\Scripts\activate
    uvicorn main:app --reload
    ```

  - **Terminal 2 → Frontend**
    ```bash
    cd frontend-folder
    npm start
    ```

Now both backend & frontend are running 🎉

---

## 🛠️ Tech Stack

- **Backend**: FastAPI, Uvicorn, NLTK, Flask (legacy), Gunicorn  
- **Frontend**: React, React-Scripts (CRA), TailwindCSS, Axios, Lucide-React  

---

## 📌 Notes

- Ensure `models/deepfake_model.h5` is placed in the correct folder (`/models/`).  
- You may need to download NLTK datasets if used in `deepfake_detector.py`:
  ```python
  import nltk
  nltk.download('punkt')
  nltk.download('stopwords')
  ```

---

✅ You're all set! Run the backend & frontend and start using the Deepfake Detection Project.
