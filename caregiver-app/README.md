# Caregiver App — Synergy Demo

## What It Does
This web app acts as a **caregiver monitoring dashboard**. It displays 6 live patient health and environmental readings by listening in real time to a shared Firebase Realtime Database.

- **Monitored Metrics**:
  - `eda`: Electrodermal Activity (µS)
  - `bvm`: Blood Volume Monitor
  - `roomTemp`: Room Temperature (°C)
  - `roomHumidity`: Room Humidity (%)
  - `envTemp`: Environmental Temperature (°C)
  - `envHumidity`: Environmental Humidity (%)

- **User Status Alerts**:
  - `⚠️ Patient App is Not Responding`: Triggered if no database update is received for over 30 seconds.
  - `📡 No Signal from Wristband`: Triggered if no database update is received for 15-30 seconds.
  - `🔋 Low Battery Alert`: Triggered if wristband battery drops below 20%.
  - `⌚ Wristband is Off`: Triggered if the wristband is disconnected from the wrist.

## How to Run
1. Open `caregiver.html` in any browser.
2. It connects to Firebase and starts displaying data.
3. If deployed to GitHub Pages, navigate to the published URL.
