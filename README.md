<div align="center">

# 🎓 SnapClass Landing Page
### Marketing site for the AI-powered classroom attendance app

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Landing%20Page-000000.svg)](https://flask.palletsprojects.com/)
[![Vercel](https://img.shields.io/badge/Deploy-Vercel-black.svg)](https://vercel.com/)

</div>

---

## 📖 About

This repository holds the **landing page** for **SnapClass**, an AI attendance system that marks a whole classroom present from a single photo or a round of spoken roll-call, using face recognition and voice biometrics.

The page introduces the product, walks through the teacher and student journeys with screenshots taken from the real app, and links visitors to the live attendance app.

- 🚀 **Live app:** [snapclass.streamlit.app](https://snapclass.streamlit.app/)
- 🧠 **Main app repository:** [Snap-Class-AI-Attendance-application-](https://github.com/Nirbhay404/Snap-Class-AI-Attendance-application-)

---

## ✨ What's on the page

| Section | Description |
| :--- | :--- |
| **Hero** | Headline, call-to-action buttons, and floating app previews |
| **Innovative Features** | AI Face Analysis, Sequential Voice ID, and QR-Driven Roster |
| **The Teacher's Journey** | Six steps: secure login, dashboard, course management, FaceID attendance, Voice ID attendance, and attendance records |
| **Advanced Tech Stack** | Streamlit and Flask, face registration, voice embeddings, Supabase |
| **The Student's Journey** | Three phases: instant enrollment, biometric registration, personal dashboard |
| **Footer** | Navigation links and branding |

Scroll-reveal animations for the cards and journey steps are in `static/js/script.js`.

---

## 🏗️ Project Structure

```text
snap-class-landing-page/
├── app.py                  # Flask server entry point
├── requirements.txt        # Flask and Gunicorn
├── vercel.json             # Vercel serverless deployment config
│
├── templates/
│   └── index.html          # The landing page template
│
└── static/
    ├── css/style.css       # Styles (Outfit and Climate Crisis fonts)
    ├── js/script.js        # Scroll-reveal interactions
    ├── fonts/chison.ttf    # Custom display font
    └── img/
        ├── logo.png        # Favicon
        ├── app_logo.png    # Navbar and footer logo
        └── demo/           # Screenshots of the SnapClass app
```

---

## 🛠️ Tech Stack

- **Backend:** [Flask](https://flask.palletsprojects.com/) serving a single Jinja template
- **Production server:** [Gunicorn](https://gunicorn.org/)
- **Styling:** Hand-written CSS with Google Fonts (*Outfit*, *Climate Crisis*)
- **Hosting:** [Vercel](https://vercel.com/) (Python serverless function)

---

## 🚀 Running Locally

### 1. Clone the repository
```bash
git clone https://github.com/Nirbhay404/snap-class-landing-page.git
cd snap-class-landing-page
```

### 2. Create a virtual environment and install dependencies
```bash
python3 -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Start the server
```bash
python app.py
```

Then open [http://localhost:5002](http://localhost:5002).

---

## 🌐 Deployment (Vercel)

1. Import this repository on [Vercel](https://vercel.com/new).
2. Leave the root directory as the repository root.
3. Vercel reads `vercel.json` and deploys `app.py` as a Python serverless function, routing every path to it.

---

## 🖼️ Updating the screenshots

The images in `static/img/demo/` are screenshots of the running SnapClass app. To refresh one, replace the file with the same name; the template references them by filename:

| File | Shows |
| :--- | :--- |
| `snap-landing.png` | App home screen |
| `snap-teacher-flow-1-login.png` | Teacher login |
| `snap-teacher-flow-2-dashboard.png` | Manage Subjects |
| `snap-teacher-flow-3-create-course.png` | Create New Subject dialog |
| `snap-teacher-flow-4-share-qr-or-link.png` | Share class link and QR code |
| `snap-teacher-flow-5.1-voice-attendance.png` | Voice attendance dialog |
| `snap-teacher-flow-5.2-photo-attendance.png` | Take AI Attendance dashboard |
| `snap-teacher-flow-5-see-stored-records.png` | Attendance records |
| `snap-student-flow-1-enroll.png` | Enroll in Subject dialog |
| `snap-student-flow-2-faceid.png` | Student FaceID login |
| `snap-student-flow-3-dashboard.png` | Student dashboard |

---

## 👨‍💻 Author

Created with ❤️ by **Nirbhay Kumar**
- GitHub: [@Nirbhay404](https://github.com/Nirbhay404)
