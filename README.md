# ALiMU Low-Grade & High-Grade IMU Dataset for End-to-End Mapping

This repository provides an **Inertial Measurement Unit (IMU) dataset** for different grading levels. It includes both **synthetic** and **real-world** IMU data collected under various scenarios.  

## Dataset Overview  

The dataset consists of:  
- **Synthetic Data**: Generated using MATLAB, simulating IMU readings under controlled conditions.  
- **Real Sensor Data**: Collected from multiple IMU sensors in different environments.  

---

## **Synthetic Data**  

The synthetic dataset is created using MATLAB and includes various motion scenarios such as:  
- **Stationary**  
- **Dynamic motion conditions**  

### **Low-Grade Synthetic IMU**  
This dataset is generated based on sensor model parameters, including Noise Density, Bias Instability (Custom), Random
Walk, Constant Bias, and Axes Misalignment at 100 HZ sampling frequency

The data is derived from the consumer-grade **ICM-20948** IMU by **TDK InvenSense** and is named as IMU-low in the paper.  
 
### **High-Grade Synthetic IMU**  
Similar sensor parameters are used for a high-grade (tactical grade) inertial sensor: Noise Density, Bias Instability, Random Walk, Constant Bias, Axes 

This data is based on the **VN-310 DUAL GNSS / INS** from **VectorNav** and is named as IMU-high in the paper.  

---

## **Real Sensor Data**  
The real sensor data is captured at 40 Hz sampling frequency. 
### **Low-Grade (Consumer-Grade) IMUs**  
The dataset includes a heterogeneous set of three low-cost MEMS-based IMUs. These IMUs exhibit differences in:
Noise levels, Drift and bias, and Temperature dependencies and are
- **BMX160** (Bosch)  
- **MPU9250** (TDK InvenSense)  
- **LSM9DS1** (STMicroelectronics)  

### **High-Grade (Industrial-Grade) IMU**  
- **VN100 IMU/AHRS** (VectorNav)  

---

## Data Format  

The dataset is provided in **CSV format**, containing synchronized sensor readings from both **low-grade** and **high-grade** IMUs.  

- **Timestamp**  
- **Accelerometer Data** (X, Y, Z) [m/s²]  
- **Gyroscope Data** (X, Y, Z) [°/s]  
- **Magnetometer Data** (X, Y, Z) [µT] 

### **CSV Structure**  

|Timestamp|Low_Acc_X|Low_Acc_Y|Low_Acc_Z|Low_Gyro_X|Low_Gyro_Y|Low_Gyro_Z|Low_Mag_X|Low_Mag_Y|Low_Mag_Z|High_Acc_X|High_Acc_Y|High_Acc_Z|High_Gyro_X|High_Gyro_Y|High_Gyro_Z|High_Mag_X|High_Mag_Y|High_Mag_Z|    
|---------|---------|---------|---------|----------|----------|----------|---------|---------|---------|----------|----------|----------|-----------|-----------|-----------|----------|----------|----------|   
| 0.001s  | 0.12    | -0.05   | 9.81    | 0.02     | -0.01    |  0.03    |  45.2   |  -30.1  |  12.7   |  0.12    |  -0.05   |  9.81    |  0.002    |  -0.001   |   0.003   |   45.2   |  -30.1   |   12.7   |   

Each row represents an IMU reading at a specific timestamp, with corresponding data from both **low-grade** and **high-grade** IMUs.  



---

## Citation  

If you use this dataset in your research, please cite our research paper. Chudamani Sahu, Shashi Poddar, ALiMU: an end-to-end mapping framework for advanced low-grade inertial measurement units, Measurement, 2025, 118736, ISSN 0263-2241, https://doi.org/10.1016/j.measurement.2025.118736.

## Reference
1. MATLAB "https://in.mathworks.com/help/nav/ref/imusensor-system-object.html"
2. VectoNav VN310 "https://www.vectornav.com/products/detail/vn-310"
3. TDK InvenSense ICM-20948 Datasheet "https://invensense.tdk.com/download-pdf/icm-20948-datasheet/"


