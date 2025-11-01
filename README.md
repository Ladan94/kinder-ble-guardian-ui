# KinderGuard BLE UI (Simulator)
**Author:** Ladan Seddighi

A single-file Streamlit app that simulates a kindergarten BLE proximity monitor with four states:
**INSIDE / WARN / OUTSIDE / LOST**. No hardware needed. Daily CSV logs included.

## Demo features
- Big state banner, live metrics (distance, RSSI, last seen)
- 3-minute sparkline
- Live event log (arrival, departure, state changes, lost)
- Adjustable thresholds (safe radius, warn margin, debounce, lost windows, EMA)
- “Silence alarms for 2 minutes” button
- Daily CSV export (e.g., `kinder_ble_YYYY-MM-DD.csv`)

## Quick start
```bash
# 1) Create a virtual environment (Python 3.11 recommended)
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

# 2) Install deps
pip install --upgrade pip
pip install -r requirements.txt

# 3) Run
streamlit run kinder_ui.py
# open http://localhost:8501
