# 🏋️ Gym-Buddy

**Gym-Buddy** is an intelligent fitness and workout companion web application built with Python and Streamlit. It leverages machine learning and computer vision detectors to assist users in tracking workouts, monitoring exercise form, and managing fitness data.

---

## ✨ Features

* **Interactive Multi-Page Dashboard:** Built with Streamlit (`pages/`), offering a clean and responsive interface for navigating workouts, analytics, and tracking tools.
* **Exercise & Pose Detection:** Integrated `detectors/` and `ml_models/` modules to analyze movement, count reps, or evaluate exercise posture.
* **Persistent Data Storage:** Uses a local SQLite database (`data.db`) to store user profiles, workout logs, and progress history.
* **Modular Architecture:** Cleanly separated `core/` and `services/` layers for scalable business logic and API/model integrations.

---

## 🛠️ Tech Stack

* **Frontend & Framework:** [Streamlit](https://streamlit.io)
* **Backend Language:** Python
* **Machine Learning & Vision:** Custom ML Models & Detectors (`ml_models/`, `detectors/`)
* **Database:** SQLite (`data.db`)

---

## 📂 Project Structure

```text
Gym-Buddy/
├── .streamlit/         # Streamlit theme and configuration settings
├── core/               # Core application logic and utilities
├── detectors/          # Computer vision / exercise detection modules
├── ml_models/          # Trained machine learning models and inference scripts
├── pages/              # Multi-page Streamlit UI views
├── services/           # External services, database handlers, and helpers
├── static/             # Static assets (images, CSS, icons)
├── .env.example        # Template for environment variables
├── data.db             # Local SQLite database
├── main.py             # Main entry point for the Streamlit app
└── requirements.txt    # Python dependencies
```

---

## 🚀 Installation & Setup

Follow these steps to run **Gym-Buddy** locally on your machine:

### 1. Clone the repository
```bash
git clone https://github.com
cd Gym-Buddy
```

### 2. Create a virtual environment (Recommended)
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure environment variables
Copy the example environment file and add your required API keys or configuration values:
```bash
cp .env.example .env
```
*(On Windows Command Prompt, use `copy .env.example .env` instead.)*

### 5. Run the application
```bash
streamlit run main.py
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com) or submit a pull request.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
