# Edge-detection using-PYNQ-Board
 ## **Overview**
This project implements the **Sobel Edge Detection algorithm** on the **PYNQ-Z2 (ZYNQ-7000)** board. The objective is to perform edge detection by combining **hardware acceleration (FPGA)** and **software (ARM processor)** capabilities. The design leverages **Vitis HLS**, **Vivado**, and **PYNQ Jupyter notebooks**.

---

## Team Members
- Umabharti H (USN: 01fe22bec209)  
- Sahana S (USN: 01fe22bec215)  
- Vaishnavi K (USN: 01fe22bec222)  
- Rakshita Gokanvi (USN: 01fe22bec236)  

**Guide:** Prof. Nikhita Patil  
**Department:** Electronics and Communication Engineering  
**Project Type:** Minor Project (Review-3)  
**Team No:** 15  

---

##  Problem Statement
The implementation of the Sobel Edge Detection algorithm on the PYNQ-Z2 or ZYNQ-7020 platform. 

---

## Objective
- To Implement Sobel edge detection on PYNQ-Z2 FPGA.
- To utilize FPGA parallelism for faster image processing.
- To compare hardware vs software performance.
- To achieve  edge detection with low latency and low power consumption.

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

##  Tools & Technologies
- **Xilinx Vitis HLS**
- **Xilinx Vivado Design Suite**
- **Python (Jupyter Notebook on PYNQ)**
- **PYNQ-Z2 FPGA Board**


## Block Diagram

<p align="center">
  <img src="https://github.com/user-attachments/assets/db7432fc-1d61-4964-9087-c1fa671f81fd" alt="Sobel Algorithm" width="500"/>
  <br>
  <b>Fig 1.1 Sobel Algorithm</b>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/1a935a4a-b66a-4f85-a699-14e8918c7979" alt="Sobel Algorithm" width="500"/>
  <br>
  <b>Fig 1.2 IP Integration </b>
</p>




