# Low-Latency Real-Time Video Monitoring System

A real-time video monitoring application built in **C++ on Linux**, designed to capture video from a USB camera, encode it using **H.264 (via GStreamer)**, and stream it over **TCP/UDP** with minimal latency.

The primary focus is **low-latency streaming (<100ms)**, achieved through careful pipeline design, buffer tuning, and real-time optimizations.

---

## ✨ Features
- Capture video from USB camera devices (e.g., `/dev/video0`)
- Encode video in **H.264** using **GStreamer pipelines**
- Stream video over **TCP/UDP sockets**
- Tuned for **<100ms glass-to-glass latency**
- Configurable parameters: resolution, frame rate, bitrate
- Modular **C++ design** following OOP & SOLID principles
- Build system powered by **CMake**

---

## 🛠️ Tech Stack
- **Language:** C++17  
- **Frameworks/Libraries:**  
  - [GStreamer](https://gstreamer.freedesktop.org/) – video capture, encoding & streaming  
  - [GLib](https://developer.gnome.org/glib/) – event loop support  
- **Build System:** CMake  
- **Platform:** Linux (tested on Ubuntu 22.04)  
- **Version Control:** Git  

---

## 📦 Installation

### Prerequisites
Make sure you have the following installed:
```bash
sudo apt-get update
sudo apt-get install build-essential cmake git pkg-config \
    libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev \
    gstreamer1.0-plugins-good gstreamer1.0-plugins-bad \
    gstreamer1.0-plugins-ugly gstreamer1.0-libav
