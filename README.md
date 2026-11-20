<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/header-light.svg" />
  <img src="./assets/header-dark.svg" width="100%" alt="Jed B. Padro. Computer Engineering student at Southern Leyte State University, building practical systems across software and hardware. Open to software engineering internships." />
</picture>

<p align="center">
  <a href="https://www.linkedin.com/in/jed-padro-ba9563299/"><img src="https://img.shields.io/badge/LinkedIn-8B1E2D?style=flat-square&logo=linkedin&logoColor=white" height="26" alt="LinkedIn" /></a>
  <a href="mailto:jedpadro@gmail.com"><img src="https://img.shields.io/badge/Email-8B1E2D?style=flat-square&logo=gmail&logoColor=white" height="26" alt="Email" /></a>
  <a href="https://jeedp.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-8B1E2D?style=flat-square&logo=googlechrome&logoColor=white" height="26" alt="Portfolio" /></a>
</p>

## About

I'm Jed Padro, a 4th-year Computer Engineering student at Southern Leyte State University in the Philippines, working toward a career in software engineering.

Most of what I build sits where software meets hardware: firmware on an ESP32, a server on a Raspberry Pi, and the interface people actually use. I care about systems that keep working outside the lab, and I document them well enough that someone else can run them.

## Featured projects

### [SLSU Campus Wayfinding System](https://github.com/cymrcsm/slsu-map-navigation)

<sub>THESIS · TEAM OF TWO · IN PROGRESS</sub>

An offline touchscreen kiosk that helps students and visitors find buildings, offices, and facilities on the SLSU main campus, with a 2D vector map, floor plans, and walking directions.

- Cut the floor drawings from 14 MB to 1.5–3 MB each so the map runs smoothly on a Raspberry Pi 4
- Built the QR hand-off that continues a route on a visitor's phone with live GPS
- Wrote the setup script and guide that turn a blank Raspberry Pi card into a working kiosk

<samp>JavaScript · Node.js · Express · SQLite · HTML/CSS · Raspberry Pi</samp>

<details>
<summary><sub>How it works</sub></summary>

```mermaid
flowchart LR
  K["Touchscreen<br/>(Chromium kiosk mode)"] --> S["Node.js + Express<br/>on Raspberry Pi"]
  S --> D[("SQLite<br/>settings and overrides")]
  S --> M["Vector map, floor plans<br/>and walking paths"]
  K -- "QR code" --> P["Visitor's phone<br/>live-GPS walking map"]
```

The map, floor plans, and routes are served from the Pi itself, so the kiosk keeps working without internet. Phones get the route over the kiosk's own Wi-Fi, or from a public copy of the map when they are on mobile data. The repository is hosted on [@cymrcsm](https://github.com/cymrcsm)'s account.

</details>

### [Smart Parking Gate System](https://github.com/jeedp/Smart-Parking-Gate-System)

<sub>IOT · SOLO</sub>

A parking gate that admits RFID card holders, tracks free slots with ultrasonic sensors, and reports both to a live web dashboard.

- Wrote the ESP32 firmware as FreeRTOS tasks on separate cores, so network updates never hold up the gate
- Built the dashboard: live slot count and event log from Firebase, and gate control from the browser over Bluetooth
- Added unit tests for the gate and RFID logic

<samp>C++ · ESP32 · FreeRTOS · PlatformIO · Firebase · Bluetooth LE · JavaScript</samp>

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

</details>

### [TrainSMART](https://github.com/jeedp/TrainSMARTApp)

<sub>DESKTOP · SOLO</sub>

A desktop application for workout templates, exercise management, workout tracking, and body measurements, with user accounts and a relational data model on SQL Server.

<samp>C# · Windows Forms · .NET Framework · SQL Server</samp>

<details>
<summary><sub>Also built</sub></summary>

- [**Portfolio site**](https://jeedp.github.io/portfolio/) — a responsive personal site in plain HTML, CSS, and JavaScript, with light and dark modes
- **Task Manager** — a task tracking web app in Laravel <sub>(private repository)</sub>
- [**LoginSystem**](https://github.com/jeedp/LoginSystem) and [**Calculator**](https://github.com/jeedp/Calculator) — early C# Windows Forms projects

</details>

## Tech stack

<p>
  <samp>languages&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=c,cpp,cs,py,js,php&theme=dark" height="34" alt="C, C++, C#, Python, JavaScript, PHP" />
</p>
<p>
  <samp>web&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=html,css,laravel,nodejs&theme=dark" height="34" alt="HTML, CSS, Laravel, Node.js" />
</p>
<p>
  <samp>databases&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=mysql,firebase&theme=dark" height="34" alt="MySQL, Firebase" />&nbsp;<img align="center" src="https://img.shields.io/badge/SQL%20Server-8B1E2D?style=flat-square" height="24" alt="SQL Server" />
</p>
<p>
  <samp>embedded&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=arduino,raspberrypi&theme=dark" height="34" alt="Arduino, Raspberry Pi" />&nbsp;<img align="center" src="https://img.shields.io/badge/ESP32-8B1E2D?style=flat-square&logo=espressif&logoColor=white" height="24" alt="ESP32" />
</p>
<p>
  <samp>tools&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=git,github,vscode,visualstudio,postman&theme=dark" height="34" alt="Git, GitHub, VS Code, Visual Studio, Postman" />&nbsp;<img align="center" src="https://img.shields.io/badge/Arduino%20IDE-8B1E2D?style=flat-square&logo=arduino&logoColor=white" height="24" alt="Arduino IDE" />
</p>

## GitHub activity

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://github-stats-extended.vercel.app/api?username=jeedp&show_icons=true&hide_rank=true&hide=issues%2Ccontribs&hide_border=true&border_radius=12&custom_title=GitHub%20activity&bg_color=FBF9F7&title_color=1B1416&text_color=1B1416&icon_color=8B1E2D" />
  <img src="https://github-stats-extended.vercel.app/api?username=jeedp&show_icons=true&hide_rank=true&hide=issues%2Ccontribs&hide_border=true&border_radius=12&custom_title=GitHub%20activity&bg_color=16181D&title_color=F2EEEA&text_color=F2EEEA&icon_color=D2566A" height="150" alt="GitHub statistics for jeedp: stars, commits in the last year, and pull requests." />
</picture>
<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://github-stats-extended.vercel.app/api/top-langs/?username=jeedp&layout=compact&langs_count=6&hide_border=true&border_radius=12&custom_title=Most-used%20languages&bg_color=FBF9F7&title_color=1B1416&text_color=1B1416" />
  <img src="https://github-stats-extended.vercel.app/api/top-langs/?username=jeedp&layout=compact&langs_count=6&hide_border=true&border_radius=12&custom_title=Most-used%20languages&bg_color=16181D&title_color=F2EEEA&text_color=F2EEEA" height="150" alt="Most-used languages across repositories owned by jeedp." />
</picture>

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://streak-stats.demolab.com?user=jeedp&hide_border=true&border_radius=12&background=FBF9F7&ring=8B1E2D&fire=8B1E2D&currStreakLabel=8B1E2D&sideLabels=1B1416&currStreakNum=1B1416&sideNums=1B1416&dates=6A5F61&stroke=E6DEDA" />
  <img src="https://streak-stats.demolab.com?user=jeedp&hide_border=true&border_radius=12&background=16181D&ring=D2566A&fire=D2566A&currStreakLabel=D2566A&sideLabels=F2EEEA&currStreakNum=F2EEEA&sideNums=F2EEEA&dates=A39C99&stroke=2A2D33" height="150" alt="GitHub contribution streak for jeedp: total contributions, current streak, and longest streak." />
</picture>

<sub>Live cards from [GitHub Stats Extended](https://github.com/stats-organization/github-stats-extended) and [GitHub Readme Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats). Languages count only repositories I own, so my JavaScript thesis work, hosted on a teammate's account, does not appear.</sub>

## Currently learning

- **Software engineering practices** — testing, code review, and maintainable architecture
- **Data engineering** — storage, pipelines, and how data moves between systems
- **Systems development** — designing hardware and software as one system
- **AI and machine learning** — not started yet; the next area I plan to study

## Connect

Open to software engineering internships and collaborations.

[jedpadro@gmail.com](mailto:jedpadro@gmail.com) · [LinkedIn](https://www.linkedin.com/in/jed-padro-ba9563299/) · [Portfolio](https://jeedp.github.io/portfolio/) · [GitHub](https://github.com/jeedp)
