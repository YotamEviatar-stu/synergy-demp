# Patient App — Synergy Demo

## What It Does
This web app **simulates a patient wearing health and environmental sensors**. It generates realistic readings for 6 specific metrics every 3 seconds and writes them to a shared Firebase Realtime Database.

- **Simulated Metrics**:
  - `eda`: Electrodermal Activity (µS)
  - `bvm`: Blood Volume Monitor
  - `roomTemp`: Room Temperature (°C)
  - `roomHumidity`: Room Humidity (%)
  - `envTemp`: Environmental Temperature (°C)
  - `envHumidity`: Environmental Humidity (%)

- **Automatic threshold detection**: If localized environment temp exceeds 38.0°C OR EDA exceeds 9.0 µS, the app sets `alert: true` in the database.
- **Force Alert button**: Manually forces the high-risk alert status.
- **Demo Status Controls**: Toggle wristband connection, drain battery to test warning alerts, or trigger a full app freeze (crash).

## How to Run
1. Open `patient.html` in any browser.
2. The simulation starts automatically.
3. If deployed to GitHub Pages, navigate to the published URL.
