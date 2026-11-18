<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/hero-light.svg" />
  <img src="./assets/hero.svg" width="100%" alt="Jed B. Padro — Computer Engineering student at Southern Leyte State University. Software engineer in the making, hardware-literate by training." />
</picture>

<p align="center">
  <a href="mailto:jedpadro@gmail.com"><code>✉&nbsp;jedpadro@gmail.com</code></a>&nbsp;
  <a href="https://www.linkedin.com/in/jed-padro-ba9563299/"><code>in/jed-padro</code></a>&nbsp;
  <a href="https://github.com/jeedp?tab=repositories"><code>⌥&nbsp;repositories</code></a>
</p>

I'm **Jed Padro**, a 4th-year Computer Engineering student at Southern Leyte State University, developing toward a career in **software engineering and emerging technologies**. My degree taught me how machines work from the circuit up; my projects are where I learn to write software people can rely on.

> <samp>now&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</samp> finishing my thesis, the SLSU Campus Wayfinding System<br />
> <samp>learning&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</samp> software engineering practices, data engineering, systems development<br />
> <samp>curious&nbsp;about&nbsp;&nbsp;</samp> AI and machine learning — not started yet, next on my list<br />
> <samp>looking&nbsp;for&nbsp;&nbsp;&nbsp;&nbsp;</samp> a software engineering internship

<img src="./assets/divider.svg" width="100%" alt="" />

### <samp>01 — selected work</samp>

<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/cover-wayfinding-light.svg" />
  <img src="./assets/cover-wayfinding.svg" width="100%" alt="Campus Wayfinding — offline touchscreen kiosk for the SLSU main campus. Thesis, team of two, in progress." />
</picture>

**[SLSU Campus Wayfinding System](https://github.com/cymrcsm/slsu-map-navigation)** — a touchscreen kiosk that helps students and visitors find any building, office, or facility on campus. It runs fully offline on a Raspberry Pi, with a custom 2D vector map, office search, floor plans, and walking directions.

<details>
<summary><samp>what I worked on</samp></summary>

<br />

- **Making it run well on a Pi** — shrank and re-encoded the floor drawings (14 MB → 1.5–3 MB per floor) and lightened map zooming so it stays smooth on a Raspberry Pi 4
- **Phone hand-off** — scan a QR code at the kiosk and the route continues on your phone as a live-GPS walking map
- **Deployment** — one re-runnable script that turns a fresh Raspberry Pi OS card into the kiosk, including its own Wi-Fi network, plus the setup guide the team works from
- **Kiosk details** — an on-screen keyboard, walking time and distance on each route, and an idle screensaver that resets the kiosk for the next visitor

Built with a teammate; the repository is hosted on [@cymrcsm](https://github.com/cymrcsm)'s account.

</details>

<samp>JavaScript · Node.js · Express · SQLite · HTML/CSS · Raspberry Pi</samp>

<br />

<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/cover-parking-light.svg" />
  <img src="./assets/cover-parking.svg" width="100%" alt="Smart Parking Gate — RFID gate with live slot tracking and a web dashboard. IoT, solo project." />
</picture>

**[Smart Parking Gate System](https://github.com/jeedp/Smart-Parking-Gate-System)** — a parking gate that knows who is allowed in and how many slots are left, and reports both to a live web dashboard. The project where I worked on every layer, from pin mapping to the browser.

<details>
<summary><samp>what I built</samp></summary>

<br />

- **Firmware** — ESP32 code split into modules for the gate, RFID reader, ultrasonic sensors, buzzer, and display, with gate control, sensing, and dashboard updates running as separate FreeRTOS tasks
- **Gate control** — RFID cards open the entry gate; servos drive entry and exit, with a 16×2 LCD showing status at the gate
- **Dashboard** — real-time slot availability over Firebase, with manual gate control from the browser and a Bluetooth fallback
- **Tests** — unit tests for the gate and RFID logic alongside the firmware

</details>

<samp>C++ · ESP32 · FreeRTOS · PlatformIO · Bluetooth LE · Firebase · JavaScript</samp>

<br />

<picture>
  <source media="(prefers-color-scheme: light)" srcset="./assets/cover-trainsmart-light.svg" />
  <img src="./assets/cover-trainsmart.svg" width="100%" alt="TrainSMART — desktop app for planning and tracking workouts. Desktop, solo project." />
</picture>

**[TrainSMART](https://github.com/jeedp/TrainSMARTApp)** — a desktop app for planning workouts and tracking progress over time. An earlier project, and the one that taught me to structure an application around its database.

<details>
<summary><samp>what I built</samp></summary>

<br />

- Workout templates and exercise management
- Workout tracking and body measurements
- User accounts with login and input validation
- Relational data model written in T-SQL on SQL Server

</details>

<samp>C# · Windows Forms · .NET Framework · SQL Server</samp>

<br />

<details>
<summary><samp>also built</samp></summary>

<br />

- **Task Manager** — a task tracking web app in Laravel, with database migrations, seeders, and Blade views <sub>(private repository)</sub>
- **[LoginSystem](https://github.com/jeedp/LoginSystem)** and **[Calculator](https://github.com/jeedp/Calculator)** — early C# Windows Forms projects where I learned UI and database basics

</details>

<img src="./assets/divider.svg" width="100%" alt="" />

### <samp>02 — toolbox</samp>

<p>
  <samp>languages&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=c,cpp,cs,py,js,php&theme=dark" height="36" alt="C, C++, C#, Python, JavaScript, PHP" />
</p>
<p>
  <samp>web&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=html,css,laravel,nodejs&theme=dark" height="36" alt="HTML, CSS, Laravel, Node.js" />
</p>
<p>
  <samp>databases&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=mysql,firebase&theme=dark" height="36" alt="MySQL, Firebase" />&nbsp;
  <img align="center" src="https://img.shields.io/badge/SQL%20Server-800000?style=for-the-badge" height="36" alt="SQL Server" />
</p>
<p>
  <samp>embedded&nbsp;&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=arduino,raspberrypi&theme=dark" height="36" alt="Arduino, Raspberry Pi" />&nbsp;
  <img align="center" src="https://img.shields.io/badge/ESP32-800000?style=for-the-badge&logo=espressif&logoColor=white" height="36" alt="ESP32" />
</p>
<p>
  <samp>tools&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</samp>
  <img align="center" src="https://skillicons.dev/icons?i=git,github,vscode,visualstudio,postman&theme=dark" height="36" alt="Git, GitHub, VS Code, Visual Studio, Postman" />&nbsp;
  <img align="center" src="https://img.shields.io/badge/Arduino%20IDE-800000?style=for-the-badge&logo=arduino&logoColor=white" height="36" alt="Arduino IDE" />
</p>

<img src="./assets/divider.svg" width="100%" alt="" />

### <samp>03 — how I work</samp>

- **I build the whole path.** Sensor, firmware, database, dashboard — I'd rather understand every layer than hand one off as a black box.
- **I design for the hardware I actually have.** When our campus map stuttered on a Raspberry Pi, I cut each floor drawing from 14 MB to under 3 MB instead of asking for a faster board.
- **I write things down.** Setup scripts, deployment guides, and acceptance checklists, so a teammate can rebuild the system from a blank SD card without me in the room.
- **I test before the hardware arrives.** Smoke tests and laptop tooling first, so the day the device shows up is for integration, not surprises.

<img src="./assets/divider.svg" width="100%" alt="" />

### <samp>04 — currently learning</samp>

- **Software engineering practices** — testing, pull-request workflows, and architecture that stays readable as a project grows
- **Data engineering** — what happens to data after it is collected: storage, pipelines, and structure
- **Systems development** — designing hardware and software as one system rather than two halves joined at the end
- **AI / machine learning** — not started yet. It's the field I'm most curious about, and I plan to begin with the fundamentals.

<details>
<summary><samp>github activity</samp></summary>

<br />

<div align="center">

<img src="https://github-stats-extended.vercel.app/api?username=jeedp&show_icons=true&hide_rank=true&hide_border=true&bg_color=120B0D&title_color=E0566A&icon_color=E0566A&text_color=F6EDE9" height="165" alt="GitHub statistics for jeedp" />
<img src="https://github-stats-extended.vercel.app/api/top-langs/?username=jeedp&layout=compact&hide_border=true&bg_color=120B0D&title_color=E0566A&text_color=F6EDE9" height="165" alt="Most used languages for jeedp" />

<img src="https://streak-stats.demolab.com?user=jeedp&hide_border=true&background=120B0D&ring=E0566A&fire=E0566A&currStreakLabel=E0566A&sideLabels=F6EDE9&currStreakNum=F6EDE9&sideNums=F6EDE9&dates=BDA7A8&stroke=3D141C" height="165" alt="GitHub streak for jeedp" />

<sub>These cards only count repositories I own. My thesis work lives in a teammate's repository, so it isn't reflected here.</sub>

</div>

</details>

<img src="./assets/divider.svg" width="100%" alt="" />

<p align="center">
  <samp>open to internships and collaborations</samp><br /><br />
  <a href="mailto:jedpadro@gmail.com"><code>✉&nbsp;jedpadro@gmail.com</code></a>&nbsp;
  <a href="https://www.linkedin.com/in/jed-padro-ba9563299/"><code>in/jed-padro</code></a>
</p>

<!-- TODO: add a portfolio link above once the site is live -->
