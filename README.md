<p align="center">
  <img src="assets/banner.png" alt="Yestin Paraguya. Student developer in embedded systems. ESP32 BLE control and FreeRTOS room monitoring. GitHub: xavieryyyyyy." width="100%">
</p>

<p align="center">
  <a href="https://github.com/xavieryyyyyy"><img src="https://img.shields.io/badge/GitHub-xavieryyyyyy-000000?style=flat-square&logo=github&logoColor=white" alt="GitHub: xavieryyyyyy"></a>
  <img src="https://img.shields.io/badge/ESP32-Embedded-202020?style=flat-square&logo=espressif&logoColor=white" alt="ESP32 embedded projects">
  <img src="https://img.shields.io/badge/C%2FC%2B%2B-Firmware-202020?style=flat-square&logo=cplusplus&logoColor=white" alt="C and C++ firmware">
  <img src="https://img.shields.io/badge/FreeRTOS-Tasks-202020?style=flat-square" alt="FreeRTOS tasks">
  <img src="https://img.shields.io/badge/Status-Learning-202020?style=flat-square" alt="Status: Learning">
</p>

<p align="center">
  <a href="#selected-projects">Projects</a> &nbsp; / &nbsp;
  <a href="#versioned-with-git">Git workflow</a> &nbsp; / &nbsp;
  <a href="#view-this-portfolio">Viewing guide</a>
</p>

I'm Yestin, a student learning IoT, embedded systems, and firmware.
I use ESP32 projects to practise working with sensors, wireless communication,
and FreeRTOS. Here I share the code, wiring, and demonstrations, along with
the Git workflow I used to build this portfolio.

<a id="selected-projects"></a>

## Selected projects

### <img src="assets/icons/radio.svg" width="24" height="24" alt=""> ESP32 Master-Slave BLE

<img src="assets/ble-system.svg" alt="Conceptual topology: one Master controls LEDs on two BLE peripherals. Not a wiring diagram." width="100%">

**One pushbutton controls LEDs on two other boards over Bluetooth Low Energy.**

My individual build includes firmware, wiring, and recorded hardware demonstrations.

- Hold the Master's button to send `ON`; release it to send `OFF`.
- Separate FreeRTOS workers handle commands for each peripheral.
- Hardware recordings and Serial Monitor logs show the individual build in action.

`ESP32` &nbsp; `BLE / GATT` &nbsp; `FreeRTOS` &nbsp; `C++`

[Source & wiring](https://github.com/xavieryyyyyy/esp32_master-slave-ble_comm) &nbsp; / &nbsp;
[Hardware & serial demonstrations](https://github.com/xavieryyyyyy/esp32_master-slave-ble_comm#demonstrations)

> The original Master is the hardware-tested reference. The modular Master still needs separate build and hardware verification.

### <img src="assets/icons/thermometer.svg" width="24" height="24" alt=""> Real-Time Room Monitoring

<img src="assets/room-system.svg" alt="Conceptual room-monitoring data path: inputs pass through ESP32 FreeRTOS tasks to the OLED and alarm. Wokwi simulation." width="100%">

**Sensor readings, an OLED display, and a temperature alarm, managed with FreeRTOS.**

The project separates sensing, user input, display updates, and alarms into
FreeRTOS tasks. Its demonstration runs in Wokwi.

- Read temperature, humidity, light, and motion inputs.
- View sensor pages on the OLED and change pages with a rotary encoder.
- Trigger a buzzer when temperature goes outside the configured limits.

`ESP32` &nbsp; `ESP-IDF` &nbsp; `FreeRTOS` &nbsp; `Wokwi`

[Source & documentation](https://github.com/xavieryyyyyy/esp32-freertos-room-monitoring-system) &nbsp; / &nbsp;
[Watch the simulation](https://youtu.be/mw-oIcxFS5U)

> The linked recording demonstrates the system in simulation; it is not a physical hardware test.

<a id="versioned-with-git"></a>

## <img src="assets/icons/git-branch.svg" width="24" height="24" alt=""> Versioned with Git

<img src="assets/git-workflow.svg" alt="Main branches into feature/profile for two improvements, then merges back before the features and tools update." width="100%">

I reviewed changes with `git diff`, selected them with `git add`, and saved each
improvement with `git commit`. The project descriptions and viewing instructions
were added on `feature/profile`, merged into `main`, and pushed to GitHub.

| Commit | What changed |
| :--- | :--- |
| `60073d5` | Added my personal introduction |
| `978b5fe` | Featured the BLE and room-monitoring projects |
| `d3601b0` | Added the status badge and viewing instructions |
| `4bb80ac` | Merged `feature/profile` into `main` |
| `7919124` | Explained portfolio features and tools |

[Explore the commit history](https://github.com/xavieryyyyyy/paraguya_github_masterclass/commits/main)

## What I'm learning

- How sensor readings move through firmware to a display or output
- How BLE devices exchange commands and FreeRTOS tasks share work
- How staging, commits, branches, and merges fit into a Git workflow

## Portfolio features

- Two featured ESP32 projects with short explanations
- Links to source code, wiring, and demonstrations
- Instructions for viewing the portfolio on GitHub or in VS Code

## Tools used

| Tool | Role in this portfolio |
| :--- | :--- |
| Markdown | Readable descriptions and links |
| Git | Commits, feature branches, and merging |
| GitHub | Hosting and sharing |
| Shields.io | Monochrome technology and status badges |
| Lucide | Line icons included as SVG images |

<a id="view-this-portfolio"></a>

## <img src="assets/icons/book-open.svg" width="24" height="24" alt=""> View this portfolio

Open either project above for its code, wiring, and demonstrations.
You can read this portfolio directly on GitHub without installing anything.

In VS Code, open `README.md` and press **Ctrl+Shift+V** to preview it.

---

[Yestin Paraguya](https://github.com/xavieryyyyyy) / Icons by [Lucide](https://lucide.dev/) ([ISC license](assets/icons/LICENSE)).
