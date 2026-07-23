<div align="center">

# 🛡️ AlertGuard
### AI-Powered Driver Drowsiness Detection & Safety Monitoring System

*Because the best accident is the one that never happens.*

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Backend-000000?style=for-the-badge&logo=flask&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-ComputerVision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-FaceMesh-00A98F?style=for-the-badge&logo=google&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio-SMS_Alerts-F22F46?style=for-the-badge&logo=twilio&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

</div>

---

## 🎯 What Is AlertGuard?

AlertGuard watches the road *through the driver's face*. Using nothing but a webcam, it continuously reads eye closure, yawning, and head position — catching fatigue in the seconds before it becomes dangerous, not after. When drowsiness is detected it sounds an alert; when it becomes critical, it texts a guardian the driver's exact live location.

<div align="center">

| 👁️ Eye Tracking | 😮 Yawn Detection | 🧭 Head Pose | 🔐 Face Login |
|:---:|:---:|:---:|:---:|
| EAR-based real-time analysis | Fatigue pattern recognition | Distraction alerts | Liveness-verified access |

</div>

---

## ✨ Features

<table>
<tr>
<td width="50%" valign="top">

### 🧠 Smart Detection
- Real-time **Eye Aspect Ratio (EAR)** tracking
- Yawn frequency analysis
- Head pose estimation for distraction
- Classifies state: `Active` → `Drowsy` → `Sleeping`

</td>
<td width="50%" valign="top">

### 🚨 Instant Response
- Audible alert on drowsiness
- Automatic **SMS + live GPS** to guardian on critical fatigue
- Timestamped logs, downloadable anytime

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 Secure Access
- Facial recognition login
- Liveness detection blocks photo/video spoofing

</td>
<td width="50%" valign="top">

### 📊 Live Dashboard
- Camera feed + EAR graph
- Color-coded driver status
- Map view, alert panel, document upload

</td>
</tr>
</table>

---

## ⚙️ How It Works

```mermaid
flowchart TD
    A[🔐 Login + Liveness Check] --> B[📊 Dashboard Loads]
    B --> C[📷 Camera Activates]
    C --> D[🧩 Facial Landmark Detection]
    D --> E[📐 Calculate EAR / Yawn / Head Pose]
    E --> F{Driver State?}
    F -->|Active| G[✅ Continue Monitoring]
    F -->|Drowsy| H[🔊 Sound Alert]
    F -->|Sleeping 7s+| I[📍 SMS + Live Location to Guardian]
    H --> J[📝 Log Event]
    I --> J
    G --> C
```

---

## 🏗️ Architecture

| Module | Role |
|---|---|
| 🔐 **Authentication** | Registration, login, liveness detection |
| 👁️ **Detection** | EAR / yawn / head-pose analysis via MediaPipe |
| 📊 **Dashboard** | Real-time visualization of all data |
| 🔔 **Alerts** | Sound warnings + Twilio SMS |
| 🗺️ **Location** | Google Maps live tracking |
| 📝 **Logs** | Timestamped records, export support |

---

## 🧰 Tech Stack

<div align="center">

`Python` `Flask` `OpenCV` `MediaPipe` `HTML/CSS/JS` `Twilio API` `Google Maps API`

</div>

---

## 🚀 Quick Start

```bash
# Clone the repo
git clone https://github.com/<your-username>/alertguard.git
cd alertguard

# Install dependencies
pip install -r requirements.txt
```

Create a `.env` file:
```env
TWILIO_ACCOUNT_SID=your_sid
TWILIO_AUTH_TOKEN=your_token
TWILIO_PHONE_NUMBER=your_number
GOOGLE_MAPS_API_KEY=your_key
```

Run it:
```bash
python app.py
```

Then open **`http://localhost:5000`** 🎉

---

## 📸 Demo

<div align="center">

<img src="assets/screenshots/login.png" width="45%" alt="Login"/> <img src="assets/screenshots/dashboard.png" width="45%" alt="Dashboard"/>

<img src="assets/screenshots/map.png" width="45%" alt="Live Location"/> <img src="assets/screenshots/sms_alert.png" width="45%" alt="SMS Alert"/>

</div>

> 💡 **Want your own screenshots here?** Create `assets/screenshots/` in your repo, drop your images in, and reference them like `assets/screenshots/dashboard.png` — GitHub renders them automatically once pushed. No repo yet? Drag an image into the GitHub web editor or a draft issue to get an instant hosted URL.

---

## 🧪 Testing

✅ Unit testing &nbsp; ✅ Integration testing &nbsp; ✅ Functional testing &nbsp; ✅ Performance testing &nbsp; ✅ Scenario-based simulation (active / drowsy / sleeping)

---

## 🗺️ Roadmap

- [ ] 🔌 Dedicated in-vehicle hardware build
- [ ] 🧠 Deep-learning models for higher accuracy
- [ ] 📳 Voice & vibration alerts, vehicle-control triggers
- [ ] ☁️ Cloud sync for logs & driving analytics
- [ ] 📱 Companion mobile app
- [ ] 🔮 Predictive fatigue warnings

---

## 👥 Team

<div align="center">

| Name | Roll No. | Division |
|---|:---:|:---:|
| Anusha Patil | 2425000174 | B-44 |
| Pratik Patil | 2425000705 | B-46 |
| Shrutika Patil | 2425001031 | B-50 |
| Adarsh Gurav | 2425000776 | B-73 |
| Sanket Magdum | 2425000540 | B-77 |

**Guide:** Mr. Chaitanya Pednekar
**Institution:** Kolhapur Institute of Technology's College of Engineering, Kolhapur *(Empowered Autonomous)*

</div>

---

## 📚 References

[OpenCV](https://opencv.org) · [MediaPipe](https://developers.google.com/mediapipe) · [Flask](https://flask.palletsprojects.com) · [Twilio](https://www.twilio.com/docs) · [Google Maps Platform](https://developers.google.com/maps)

---

<div align="center">

**Made with 🖤 for safer roads**

</div>
