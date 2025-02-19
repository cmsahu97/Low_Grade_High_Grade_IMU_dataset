# Low-Grade & High-Grade IMU Dataset  

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
This dataset is generated based on sensor model parameters, including:  
- **Noise Density**  
- **Bias Instability**  
- **Random Walk**  
- **Constant Bias**  
- **Axes Misalignment**  

The data is derived from the consumer-grade **ICM-20948** IMU by **TDK InvenSense**.  

- **IMU Model**: ICM-20948 (TDK InvenSense)  

### **High-Grade Synthetic IMU**  
Similar sensor parameters are used for a high-grade (tactical-grade) inertial sensor:  
- **Noise Density**  
- **Bias Instability**  
- **Random Walk**  
- **Constant Bias**  
- **Axes Misalignment**  

This data is based on the **VN-310 DUAL GNSS / INS** from **VectorNav**.  

- **IMU Model**: VN-310 DUAL GNSS / INS (VectorNav)  

---

## **Real Sensor Data**  

### **Low-Grade (Consumer-Grade) IMUs**  
The dataset includes a heterogeneous set of three low-cost MEMS-based IMUs:  
- **BMX160** (Bosch)  
- **MPU9250** (TDK InvenSense)  
- **LSM9DS1** (STMicroelectronics)  

These IMUs exhibit differences in:  
- Noise levels  
- Drift and bias  
- Temperature dependencies  

### **High-Grade (Industrial-Grade) IMU**  
- **VN100 IMU/AHRS** (VectorNav)  

---

## **Data Format**  

The dataset is provided in CSV format, with the following structure:  

| Timestamp | Low_Acc_X (m/s²) | Low_Acc_Y (m/s²) | Low_Acc_Z (m/s²) | Low_Gyro_X (°/s) | Low_Gyro_Y (°/s) | Low_Gyro_Z (°/s) | Low_Mag_X (µT) | Low_Mag_Y (µT) | Low_Mag_Z (µT) | High_Acc_X (m/s²) | High_Acc_Y (m/s²) | High_Acc_Z (m/s²) | High_Gyro_X (°/s) | High_Gyro_Y (°/s) | High_Gyro_Z (°/s) | High_Mag_X (µT) | High_Mag_Y (µT) | High_Mag_Z (µT) |    
|-----------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-----------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|-------------|    
| 0.001s    | 0.12       | -0.05       | 9.81        | 0.02        | -0.01       | 0.03        | 45.2        | -30.1       | 12.7        | 0.001s    | 0.12       | -0.05       | 9.81        | 0.002        | -0.001       | 0.003        | 45.2        | -30.1       | 12.7        |   

---

## **Applications**  

This dataset can be used for:  
- **Sensor Fusion & Calibration**  
- **Machine Learning for Motion Tracking**  
- **Inertial Navigation System (INS) Research**  

---

## **License**  

This dataset is made available under the **[
