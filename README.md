# 🖥️ wt32-hw-monitor - Real-Time PC Hardware Display

[![Download wt32-hw-monitor](https://img.shields.io/badge/Download-Get%20It-blue?style=for-the-badge)](https://github.com/Earthly-ankus691/wt32-hw-monitor)

---

## 📋 About wt32-hw-monitor

wt32-hw-monitor is a simple tool that shows live PC hardware data on an ESP32 WT32-SC01 touchscreen. It displays CPU, GPU, RAM, disk, network, and fan information. This project uses LibreHardwareMonitor for data gathering, Python for processing, and PlatformIO for ESP32 programming.

It works as an open-source alternative to AIDA64 sensor panels. You can track your PC's hardware status in real time without complicated setup.

---

## 🔎 Features

- Displays CPU temperature and usage  
- Shows GPU performance and temperature  
- Monitors RAM and disk usage  
- Tracks network activity  
- Shows fan speeds  
- Uses an ESP32 WT32-SC01 touchscreen for easy reading  
- Runs smoothly without affecting PC performance  
- Open-source, you can modify it if needed  

---

## 🖥️ System Requirements

- Windows 10 or newer  
- PC with LibreHardwareMonitor compatible hardware  
- ESP32 WT32-SC01 touchscreen device  
- USB cable to connect PC and ESP32 screen  
- Internet connection for software download  

---

## 🚀 Getting Started

### Step 1: Download the software

Click the link below to visit the release page and download the necessary files for Windows.

[![Download wt32-hw-monitor](https://img.shields.io/badge/Download-Get%20It-brightgreen?style=for-the-badge)](https://github.com/Earthly-ankus691/wt32-hw-monitor)

The page contains the firmware for the ESP32 device and PC software components.

### Step 2: Install the PC software

1. Download the latest Windows installer from the release page. It will install the Python scripts and LibreHardwareMonitor components needed for monitoring.

2. Run the installer by double-clicking the downloaded file.

3. Follow the on-screen instructions to complete the installation.

### Step 3: Connect the ESP32 WT32-SC01 touchscreen  

1. Use a USB cable to connect your ESP32 WT32-SC01 to your PC.

2. Make sure the device powers on and the touchscreen lights up.

### Step 4: Flash the ESP32 device  

1. Download PlatformIO, which is a tool to load the firmware on your ESP32. You can install PlatformIO inside Visual Studio Code or separately.  

2. Open the firmware file from the release page in PlatformIO.

3. Follow PlatformIO instructions to upload (flash) the firmware onto the ESP32 device.

### Step 5: Start monitoring  

1. Run the PC software installed in Step 2.

2. The software will detect the ESP32 screen connected via USB.

3. It will stream hardware data live to the ESP32 touchscreen.

4. Use the touchscreen to view your CPU, GPU, RAM, disk, network, and fan data easily.

---

## ⚙️ How it works

wt32-hw-monitor uses LibreHardwareMonitor to collect sensor data from your PC. The Python scripts fetch this data and send it over to the ESP32 WT32-SC01 device. The ESP32 writes the information on its touchscreen in real time.

The system updates every second to give you fresh data. It uses a simple, clear interface optimized for the small screen.

---

## 🛠 Troubleshooting

### The ESP32 device does not show data  

- Check the USB cable connection and power status.  
- Make sure you flashed the firmware correctly with PlatformIO.  
- Verify the PC software is running and detects the device.  
- Restart both PC software and ESP32 device.  

### PC software fails to install or run  

- Ensure you are on Windows 10 or later.  
- Confirm you have administrator rights during installation.  
- Check if any security software blocks the installer or Python scripts.  
- Re-download the installer to avoid corrupted files.  

### Data on the screen looks incorrect or frozen  

- Restart the PC software and the ESP32 device.  
- Verify internet and USB connections remain stable.  
- Confirm LibreHardwareMonitor is running without errors.  

---

## 💡 Tips for Best Use

- Place the ESP32 touchscreen in a convenient spot near your PC for quick monitoring.  
- Keep your PC software updated using the GitHub release page.  
- Use the touchscreen controls to switch between hardware categories if supported.  
- Close other programs that use large CPU or network resources to get accurate readings.  

---

## 🔗 Useful Links

- Visit the main page to download and find new updates:  
  https://github.com/Earthly-ankus691/wt32-hw-monitor  

- Information on the hardware used:  
  ESP32 WT32-SC01 touchscreen  

- PlatformIO installation and instructions:  
  https://platformio.org/install  

- LibreHardwareMonitor project page for troubleshooting and details:  
  https://github.com/LibreHardwareMonitor/LibreHardwareMonitor  

---

## 📂 File Structure Overview

After installation, you will find these important files on your PC:

- `wt32_hw_monitor.exe` – The main Windows executable for data streaming and interface  
- `config.json` – Settings file where you can adjust connection options  
- `firmware.bin` – ESP32 firmware to flash on your touchscreen device  
- `libs/` – Supporting libraries for LibreHardwareMonitor and Python scripts  

---

## 🛡 Privacy and Data Use

The software only collects local hardware sensor data. It does not send your information to any external servers. All data stays on your PC and ESP32 device. You control what is displayed.

---

## 🔧 Customization

If you want to change what hardware data is shown:

- Edit the Python scripts in the installation folder.  
- Adjust the sensor selection in `config.json`.  
- Rebuild and flash the ESP32 firmware to see interface changes.  
  
This requires basic knowledge of Python and PlatformIO but allows full control over functionality.

---

## 💻 Development Notes

wt32-hw-monitor is built with:

- Python 3.x for handling PC data processing  
- LibreHardwareMonitor as the sensor source  
- PlatformIO framework to program the ESP32 WT32-SC01 device  
- LovyanGFX library for ESP32 touchscreen display rendering  

This modular design keeps data collection, processing, and display separate for easier updates.

---

## 🎯 Keywords / Topics  

arduino, cpu-temperature, diy-electronics, esp32, esp32-project, gpu-monitor, hardware-monitor, librehardwaremonitor, lovyangfx, pc-monitoring, platformio, sensor-panel, system-monitor, touchscreen, wt32-sc01