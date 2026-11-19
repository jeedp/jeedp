<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/annual-cover-light.svg" />
  <img src="./assets/annual-cover-dark.svg" width="100%" alt="Annual report cover for Jed B. Padro, BS Computer Engineering, Southern Leyte State University. 158 contributions on 22 active days in the last twelve months, three featured projects, on GitHub since 2024, and a bar chart of contributions per month." />
</picture>

**Jed B. Padro** · BS Computer Engineering, Southern Leyte State University  
Computer Engineering student building practical systems across software and hardware.

[jedpadro@gmail.com](mailto:jedpadro@gmail.com) · [LinkedIn](https://www.linkedin.com/in/jed-padro-ba9563299/) · [Portfolio](https://jeedp.github.io/portfolio/) · [Repositories](https://github.com/jeedp?tab=repositories)

**Summary.** I'm a 4th-year Computer Engineering student in the Philippines working toward a career in software engineering. My projects tend to sit where software meets hardware: firmware on an ESP32, a server on a Raspberry Pi, and the interface people actually use.

**Outlook.** Completing my thesis, the SLSU Campus Wayfinding System, then looking for a software engineering internship.

#### Highlights

- Reduced the thesis kiosk's floor drawings from 14 MB to 1.5–3 MB per floor so the campus map runs smoothly on a Raspberry Pi 4.
- Built the Smart Parking Gate end to end: ESP32 firmware, RFID and ultrasonic sensing, a live Firebase dashboard, and gate control from the browser over Bluetooth.
- Split the parking gate's firmware into FreeRTOS tasks on separate ESP32 cores, keeping gate control apart from network updates.
- Wrote the deployment script and setup guide that turn a blank Raspberry Pi card into a working kiosk.

#### Key figures

<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/annual-figures-light.svg" />
  <img src="./assets/annual-figures-dark.svg" width="100%" alt="Key figures for the twelve months to 18 Nov 2026: 158 contributions, 151 commits, 4 pull requests, 22 active days, busiest day 26 contributions. Language share across own public repositories: C# 57%, T-SQL 21%, HTML 8%, C++ 7%, other 7%." />
</picture>

<details>
<summary><sub>Notes to the figures</sub></summary>

- **Period:** the twelve months to 18 November 2026, as GitHub counts public contributions (commits, pull requests, issues and reviews). Figures are a snapshot taken on that date and are not updated automatically.
- **Contributions** include work in repositories owned by others, such as the thesis repository.
- **Languages** are measured only across repositories I own, so they lean toward my earlier C# projects and leave out the JavaScript thesis work.

<sub>Layout based on the Annual Report template from [README Templates](https://github.com/Dr-At0mic/README-Templates). Motion stops if your system asks for reduced motion.</sub>

</details>

#### Portfolio

**[SLSU Campus Wayfinding System](https://github.com/cymrcsm/slsu-map-navigation)** · Thesis · team of two · in progress  
An offline touchscreen kiosk that helps students and visitors find buildings, offices, and facilities on the SLSU main campus, with a 2D vector map, floor plans, and walking directions.

- **My part:** performance on the Raspberry Pi (floor drawings cut from 14 MB to 1.5–3 MB each), the QR hand-off that continues a route on a visitor's phone with live GPS, and the setup script and guide for deploying the kiosk.
- **Stack:** JavaScript, Node.js, Express, SQLite, HTML/CSS, Raspberry Pi

<details>
<summary><sub>How it works</sub></summary>

```mermaid
flowchart LR
  K["Touchscreen<br/>(Chromium kiosk mode)"] --> S["Node.js + Express<br/>on Raspberry Pi"]
  S --> D[("SQLite<br/>settings and overrides")]
  S --> M["Vector map, floor plans<br/>and walking paths"]
  K -- "QR code" --> P["Visitor's phone<br/>live-GPS walking map"]
  S -. "kiosk's own Wi-Fi" .-> P
```

- **Runs without internet.** The map, floor plans, and routes are served from the Pi itself, so the kiosk keeps working if the campus network drops.
- **Phones get the route two ways:** over the kiosk's own Wi-Fi network, or from a public copy of the map for phones on mobile data.
- **Live GPS needs HTTPS,** so the kiosk serves the phone page over a trusted certificate rather than plain HTTP.

The repository is hosted on [@cymrcsm](https://github.com/cymrcsm)'s account.

</details>

**[Smart Parking Gate System](https://github.com/jeedp/Smart-Parking-Gate-System)** · IoT · solo  
A parking gate that admits RFID card holders, tracks free slots with ultrasonic sensors, and reports both to a live web dashboard.

- **My part:** all of it, from pin mapping and firmware to the dashboard, including unit tests for the gate and RFID logic.
- **Stack:** C++, ESP32, FreeRTOS, PlatformIO, Firebase, Bluetooth LE, JavaScript

<details>
<summary><sub>How it works</sub></summary>

```mermaid
flowchart LR
  R["RFID reader"] --> E["ESP32<br/>FreeRTOS tasks"]
  U["Ultrasonic sensors"] --> E
  E --> G["Entry and exit servos<br/>16×2 LCD"]
  E -- "status and event log" --> F[("Firebase<br/>Realtime Database")]
  F --> W["Web dashboard"]
  W -- "open / close over Bluetooth LE" --> E
```

- **Gate control and network updates run as separate tasks on separate cores,** so a slow connection to Firebase does not hold up the gate.
- **Manual control goes straight to the ESP32 over Bluetooth,** so an operator can open or close the gate from the browser without the internet.
- **The dashboard only reads from Firebase:** live slot count, gate state, and the last 20 events.

</details>

**[TrainSMART](https://github.com/jeedp/TrainSMARTApp)** · Desktop · solo  
A desktop application for workout templates, exercise management, workout tracking, and body measurements.

- **My part:** the full application, including user accounts with input validation and a relational data model written in T-SQL.
- **Stack:** C#, Windows Forms, .NET Framework, SQL Server

#### Capabilities

| Area | Technologies |
| :-- | :-- |
| Languages | <img src="https://skillicons.dev/icons?i=c,cpp,cs,py,js,php&theme=dark" height="32" alt="C, C++, C#, Python, JavaScript, PHP" /> |
| Web | <img src="https://skillicons.dev/icons?i=html,css,laravel,nodejs&theme=dark" height="32" alt="HTML, CSS, Laravel, Node.js" /> |
| Databases | <img src="https://skillicons.dev/icons?i=mysql,firebase&theme=dark" height="32" alt="MySQL, Firebase" /> <img src="https://img.shields.io/badge/SQL%20Server-13213B?style=flat-square" height="24" alt="SQL Server" /> |
| Embedded | <img src="https://skillicons.dev/icons?i=arduino,raspberrypi&theme=dark" height="32" alt="Arduino, Raspberry Pi" /> <img src="https://img.shields.io/badge/ESP32-13213B?style=flat-square&logo=espressif&logoColor=white" height="24" alt="ESP32" /> |
| Tools | <img src="https://skillicons.dev/icons?i=git,github,vscode,visualstudio,postman&theme=dark" height="32" alt="Git, GitHub, VS Code, Visual Studio, Postman" /> <img src="https://img.shields.io/badge/Arduino%20IDE-13213B?style=flat-square&logo=arduino&logoColor=white" height="24" alt="Arduino IDE" /> |

#### Development

- **Software engineering practices** — testing, code review, and maintainable architecture.
- **Data engineering** — storage, pipelines, and how data moves between systems.
- **Systems development** — designing hardware and software as one system.
- **AI and machine learning** — not started yet; the next area I plan to study.

<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/annual-closing-light.svg" />
  <img src="./assets/annual-closing-dark.svg" width="100%" alt="Closing note: Open to internships and collaborations. Jed B. Padro, BS Computer Engineering, Southern Leyte State University." />
</picture>
