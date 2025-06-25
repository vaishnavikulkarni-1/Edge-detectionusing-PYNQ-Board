# Edge-detection using-PYNQ-Board
 ## **Overview**
This project implements the **Sobel Edge Detection algorithm** on the **PYNQ-Z2 (ZYNQ-7000)** board. The objective is to perform real-time edge detection by combining **hardware acceleration (FPGA)** and **software (ARM processor)** capabilities. The design leverages **Vitis HLS**, **Vivado**, and **PYNQ Jupyter notebooks**.

---

## 🧠 Team Members
- Umabharti H (USN: 01fe22bec209)  
- Sahana S (USN: 01fe22bec215)  
- Vaishnavi K (USN: 01fe22bec222)  
- Rakshita Gokanvi (USN: 01fe22bec236)  

**Guide:** Prof. Nikhita Patil  
**Department:** Electronics and Communication Engineering  
**Project Type:** Minor Project (Review-3)  
**Team No:** 15  

---

## 📌 Problem Statement
To implement the **Sobel Edge Detection algorithm** on the **ZYNQ-7000 platform** (PYNQ-Z2) for detecting sharp intensity variations in images, with the aim of achieving **real-time performance** using **FPGA parallelism**.

---

## 🎯 Need Statement
- Use hardware acceleration to improve performance compared to traditional software methods.
- Utilize the FPGA’s parallel capabilities to enable real-time edge detection.
- Applications include **video processing**, **object detection**, and **autonomous systems**.

---

## ⚙️ Implementation Steps

### 1. Sobel Filter IP Creation
- Design Sobel filter in **C++** using **Vitis HLS**
- Convert to IP core for hardware integration

### 2. IP Integration in Vivado
- Setup ZYNQ processing system
- Integrate custom Sobel IP with pre-existing IP blocks
- Generate bitstream (`.bit` file)

### 3. PYNQ Board Control
- Use **Jupyter Notebook** to access and control the board
- Input image → Grayscale → Gaussian → Sobel (Gx, Gy) → Thresholding → Output edge image

---

## 🔬 Tools & Technologies
- **Xilinx Vitis HLS**
- **Xilinx Vivado Design Suite**
- **Python (Jupyter Notebook on PYNQ)**
- **PYNQ-Z2 FPGA Board**

