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

<p align="center">
  <img src="https://github.com/user-attachments/assets/68fb2c1f-7338-4cf2-8487-d5881d04141f" alt="Sobel Algorithm" width="500"/>
  <br>
  <b>Fig 1.2 IP Integration </b>
</p>

## 🛠️ Vitis HLS Design

For the Sobel algorithm to be implemented on the **PYNQ board**:

1. A custom **Intellectual Property (IP) block** was designed using **Vitis HLS** in the C++ programming language.
2. This approach simplifies the implementation of the Sobel algorithm, avoiding the need to write Verilog or VHDL manually.

   
   <p align="center">
  <img src="https://github.com/user-attachments/assets/02ee6a5a-3735-4830-919e-bf8e473d5c1d" alt="Sobel Algorithm" width="500"/>
  <br>
  <b>Fig 1.2 IP Integration </b>
</p>

## Vivado Design

The **Vivado project** is set up initially to support the **PYNQ board** by using the **ZYNQ7 Processing System**.

Generally, in Vivado, programming in **VHDL** would be necessary to create logic blocks to produce a desired outcome. However, most of the work was done in **Vitis HLS**, creating the Sobel IP.

The **Sobel IP** can then be implemented alongside other pre-made IPs and connected to the Processing System.

Vivado also provides features to assist in routing and connecting the logic blocks together.

<p align="center">
  <img src="https://github.com/user-attachments/assets/77e3681f-ecee-4e69-bc4f-2f55c9d1e5f7" alt="Vivado Block Design" width="600"/>
  <br>
  <b>Fig 1.3: Vivado Block Design for Sobel IP Integration</b>
</p>


## 📈 Results
- Demonstrated successful edge detection on input images
- Hardware implementation shows faster performance compared to software-only approaches
  
<p align="center">
  <img src="https://github.com/user-attachments/assets/cbcc6f84-48c5-4251-9d35-f45a1d5254ec" alt="Vivado Block Design" width="600"/>
  <br>
  <b>Fig 1.3: Vivado Block Design for Sobel IP Integration</b>
</p>



