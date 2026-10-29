# 💗 Family Pulse | نبض الأسرة
> **One Tap Daily Well-Being for UAE Homes**
> *Developed for Al Andalus Private Academy • أكاديمية الأندلس الخاصة*

![Family Pulse Banner](https://img.shields.io/badge/Status-Active_Prototype-10b981?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Hardware-ESP32-orange?style=for-the-badge)

---

## 📖 Overview

**Family Pulse** is a low-friction emotional wellness tracking system designed specifically for UAE households. Busy daily schedules often leave little time to ask *"How are you, really?"*. 

Family Pulse solves this by providing a non-intrusive **one-tap daily check-in routine**. Family members log their mood in seconds via a web interface or an offline physical tabletop robot placed in the living room. The system calculates an aggregated **Family Pulse Score**, detects fatigue trends, and delivers gentle, actionable recommendations to support family cohesion without privacy invasion.

---

## ✨ Key Features

* **⚡ Single-Tap Mood Check-In:** Choose a role (*Parent, Teen, Child, Grandparent*) and select 1 of 5 expressive mood states. Zero typing or questionnaires required.
* **📊 Live Pulse Dashboard:** Real-time visual gauge displaying a 0–100 aggregated family well-being score alongside historical weekly trends.
* **🧠 Smart Action Engine:** Automatically suggests low-key, culturally aligned family interventions (e.g., quiet evening tea, reducing homework stress, weekend family outings).
* **🤖 ESP32 Hardware Integration:** Low-cost tabletop physical device with tactile buttons, LED feedback, and buzzer chimes.
* **🌐 Hybrid Architecture:** Operates **100% offline via a local rule engine** or optionally connects to **Claude AI** for weekly empathetic summaries.
* **🔒 Privacy by Design:** Zero camera or audio components, full user control over sharing, and anonymous role-based metrics.
* **🌍 Bilingual Support:** Fully adaptive English and Arabic (RTL) interface tailored for multi-generational homes.

---

## 🛠️ Hardware Setup (ESP32 Tabletop Robot)

The physical device code is located in [`firmware/esp32_family_pulse.ino`](./firmware/esp32_family_pulse.ino).

### Circuit Pinout Guide:
| Component | ESP32 Pin | Description |
| :--- | :--- | :--- |
| **Member Button** | `GPIO 13` | Toggles active member |
| **Mood Buttons** | `GPIO 12, 14, 27, 26, 25` | Moods 1 (Upset) through 5 (Happy) |
| **LED 1–4** | `GPIO 15, 2, 4, 16` | Status indicators for Parent, Teen, Child, Grandparent |
| **Buzzer** | `GPIO 17` | Audio confirmation chime |

---

## 🚀 Live Demo & GitHub Pages Deployment

1. Push this repository to your GitHub account.
2. Go to **Settings** > **Pages** in your GitHub repository.
3. Under **Build and deployment** > **Branch**, select `main` and folder `/ (root)`.
4. Click **Save**. Your site will be live at `https://<your-username>.github.io/family-pulse/`.

---

## 📄 License

Distributed under the MIT License. See [`LICENSE`](./LICENSE) for details.
