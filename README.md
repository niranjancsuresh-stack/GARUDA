# G.A.R.U.D.A.

**Ground-link Automated Receiver & Unified Data Analyzer**

Plug in, test, calibrate, take data.

Created by Niranjan CS.

## What's inside

| File | What it does |
| --- | --- |
| `index.html` | The welcome pop-up: name your lab and CubeSat, then pick a section. |
| `testing-lab.html` | **CubeSat Testing Lab**: health checks, reaction wheel test, IMU and altimeter calibration. |
| `telemetry.html` | **CubeSat Telemetry**: live LoRa packets, graphs, 3D view, map, and data export. |
| `assets/garuda.js` | Shared helper: saves your names, and adds them with the date and time to every export. |
| `assets/logo-*.webp` | G.A.R.U.D.A. logos (night and day). Swap these files to change the logo. |

## Put it on GitHub Pages

1. Create a new repository on GitHub (for example `garuda`).
2. Upload everything in this folder (or unzip the archive and upload the files).
3. Go to **Settings → Pages**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then save.
4. Open the Pages link GitHub shows you. Web Serial (the USB connection) needs **Chrome or Edge** on a computer, and works on `https://` links such as GitHub Pages.

## Exports

Every download (CSV, JSON, Excel, and raw logs) includes:

- the CubeSat name and the testing lab name
- the date and time it was saved

They appear at the top of CSV and Excel files, inside JSON files under `"exported"`, and in each file name, for example `Nano-1_garuda_flight_log_2026-11-14_131522.csv`.

## Notes

- The page loads Tailwind CSS, Chart.js, SheetJS (for Excel), and the Saira font from the internet on first visit.
- Names and theme are saved in the browser on your computer. They are not sent anywhere.
