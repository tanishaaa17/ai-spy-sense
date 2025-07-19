# SpySense AI-Security Dashboard

SpySense is an **AI-powered security dashboard** for ethical hacking, monitoring, and research. It combines real-time keylogging, process detection, and system resource monitoring with Google Gemini AI to provide human-readable summaries of user activity. The dashboard features a modern, cyberpunk-inspired React UI for a true hacking simulator experience.

---

## 🚀 Features
- **AI Log Summarization:** Summarize recent keylogs into human-readable activity using Google Gemini AI.
- **Keylogging:** Capture all keystrokes with timestamps for analysis.
- **Process Detection:** Scan running processes for suspicious activity using `psutil`.
- **System Info:** Monitor CPU, RAM, and process count in real time.
- **Advanced Dashboard:** Animated, responsive React UI with hacker/cyberpunk theme, glitch effects, and integrated sidebar navigation.
- **Log Management:** Automatic log rotation and cleanup to maintain privacy and performance.

---

## 🛠️ Tech Stack
- **Backend:**
  - Python 3
  - Flask (REST API)
  - Flask-CORS (CORS support)
  - psutil (system/process info)
  - pynput (keylogging)
  - requests (Gemini API integration)
- **Frontend:**
  - React (Create React App)
  - react-icons (icons)
  - Chart.js (system monitoring charts)
  - Custom CSS (cyberpunk/hacker theme)
- **AI Integration:**
  - Google Gemini API (for log summarization)

---

## 📁 Project Structure
```
spy-sense-2/
├── backend/
│   ├── app.py             # Flask backend (API, AI, keylogger, system info)
│   ├── detector.py        # Process detection logic
│   ├── keylogger.py       # Keylogger logic
│   ├── logs.txt           # Log file (auto-generated, last 50 entries)
│   └── requirements.txt   # Backend dependencies
├── frontend/
│   ├── package.json       # Frontend dependencies and scripts
│   └── src/
│       ├── App.js         # Main React app
│       ├── Dashboard.js   # Main dashboard with integrated sidebar and all features
│       ├── Dashboard.css  # Dashboard styles with cyberpunk theme
│       ├── index.js       # React entry point
│       ├── index.css      # Global styles
│       └── ...            # Other React files/assets
├── README.md              # Project documentation
└── ...                    # .gitignore, venv, etc.
```

---

## ⚡ Setup & Usage

### 1. Clone the Repository
```bash
git clone https://github.com/tanishaaa17/ai-spy-sense.git
cd ai-spy-sense
```

### 2. Configure Your Gemini API Key
- **IMPORTANT:**
  - Open `backend/app.py` and replace the value of `GEMINI_API_KEY` with your own Google Gemini API key:
    ```python
    GEMINI_API_KEY = "YOUR_GEMINI_API_KEY"
    ```
  - [Get your Gemini API key here.](https://ai.google.dev/gemini-api/docs/quickstart)

### 3. Start the Backend
```bash
cd backend
pip install -r requirements.txt
python app.py
```
- The backend runs on [http://localhost:5000](http://localhost:5000)

### 4. Start the Frontend
```bash
cd frontend
npm install
npm start
```
- The frontend runs on [http://localhost:3000](http://localhost:3000)

---

## 🖥️ Dashboard Sections
- **Logs:** View raw keylog data (last 50 entries for privacy).
- **Gemini Summary:** See AI-generated summaries of recent user activity (last 100 keystrokes).
- **Detection:** Check for suspicious processes in real time.
- **System Info:** Monitor CPU, RAM, and process count live with interactive charts.

---

## 🔒 Privacy & Security
- **Log Rotation:** The system automatically maintains only the last 50 log entries to ensure privacy.
- **Local Processing:** All keylogging and processing happens locally on your machine.
- **No Data Collection:** No user data is sent to external servers except for AI summarization requests.

---

## 📝 Recent Updates
- **Log Management:** Implemented automatic log cleanup to maintain only recent entries
- **Repository Setup:** Connected to GitHub repository for version control
- **Privacy Enhancement:** Reduced log file size from 9,600+ entries to 50 entries
- **Documentation Update:** Corrected project structure and removed outdated component references

---

## ⚠️ Disclaimer
This project is for **educational and ethical research purposes only**. Do not use it for malicious activity. Always have permission before running keyloggers or process monitors on any system. The developers are not responsible for any misuse of this software.

---

## 🤝 Contributing
Feel free to submit issues and enhancement requests!

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details. 