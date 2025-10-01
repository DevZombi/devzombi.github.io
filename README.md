# 🏎️ Drag Strip Controller (ESP32 + Hot Wheels)

A browser-based race controller for an **ESP32-powered Hot Wheels drag strip gate system**.  
Control your drag strip from **Chrome or Edge** with just a USB cable and this webpage.

---

# ⚡ Quick Start

1. **Flash your ESP32** with `DragStripController.ino`  
   *(Install `ESP32Servo` via Arduino IDE Library Manager.)*  
2. **Open your GitHub Pages site** in Chrome/Edge.  
3. **Connect → Race!**  
   - Click **Connect** to select your ESP32  
   - Hit **Start** to drop the gates  
   - View elapsed time + live device log  

---

# ✨ Features

- Start / Stop / Reset race control  
- Elapsed time display  
- Configurable driver delays (3 presets per lane, randomly chosen)  
- 1-servo or 2-servo mode  
- Toggleable delays & race timer  
- Configurable servo gate angles  
- Clean settings modal (⚙️)  
- Live device log viewer  

---

# 🚀 How it Works

- ESP32 runs the Arduino firmware and listens for text commands over Serial.  
- This web app communicates via the **Web Serial API** (works in Chrome/Edge).  
- All commands and logs flow in real time between the ESP32 and the browser UI.  

---

# 🖥️ Usage

1. **Flash the firmware**:  
   - Open `DragStripController.ino` in Arduino IDE  
   - Install `ESP32Servo`  
   - Upload to your ESP32 board  

2. **Visit your GitHub Pages site** in Chrome/Edge.  
3. **Plug in the ESP32 via USB** and click **Connect**.  
4. Control races, adjust settings, and watch logs.  

---

# ⚙️ Commands (for reference)

- save driver1 <ms1> <ms2> <ms3>
- save driver2 <ms1> <ms2> <ms3>
- mode 1servo | mode 2servo
- delays on | delays off
- timer on | timer off
- angles s1 <up> <down>
- angles s2 <up> <down>
- start | stop | reset | status

---

# 📦 Repo Contents

- `index.html` → Web interface (served by GitHub Pages)  
- `README.md` → Documentation  

---

# 🔧 Requirements

- ESP32 board  
- Servos on pins defined in firmware (`18`, `17` by default)  
- Chrome / Edge browser with Web Serial support  

---

