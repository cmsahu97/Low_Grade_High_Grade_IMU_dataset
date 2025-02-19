# Low_Grade_High_Grade_IMU_dataset

This repository provides an Inertial Measurement Unit (IMU) dataset for different grading levels. The dataset consists of both **synthetic** and **real-world** IMU data collected under various scenarios.  

## Dataset Overview  

The dataset contains:  
- **Synthetic Data**: Generated using MATLAB to simulate IMU readings under controlled conditions.  
- **Real Sensor Data**: Collected from multiple IMU sensors in different environments.  

### Synthetic Data
The synthetic dataset is created using MATLAB, used different motion scenarios like stationary, dynamic motion condition 

#### **Low-Grade IMUs**  
The dataset is generated with different sensor model parameter like noise density,  BiasInstability, random walk, ConstantBias, AxesMisalignment, and all this data is taken from the comsumer grade ICM-20948 from TDK InvenSense
- **ICM-20948** (TDK InvenSense)  

#### **High-Grade IMU**  
The high grade (tactical-grade) inertial sensor's noise density,  BiasInstability, random walk, ConstantBias, AxesMisalignment, and all this data is taken from the comsumer grade VN-310  DUAL GNSS / INS from VectorNav 

- **VN-310  DUAL GNSS / INS** (VectorNav)  

## Data Format  

The dataset is provided in CSV format, containing:  
- **Timestamp**  
- **Accelerometer Data** (X, Y, Z) [m/s²]  
- **Gyroscope Data** (X, Y, Z) [°/s]  
- **Magnetometer Data** (X, Y, Z) [µT] 


### Real Sensor Data

#### **Low-Grade (Consumer-Grade) IMUs**  
The dataset includes a heterogeneous set of three low-cost MEMS-based IMUs:  
- **BMX160** (Bosch)  
- **MPU9250** (TDK InvenSense)  
- **LSM9DS1** (STMicroelectronics)  

These IMUs vary in signal characteristics, including:  
- Noise levels  
- Drift and bias  
- Temperature dependencies  

#### **High-Grade (Industrial-Grade) IMU**  
- **VN100 IMU/AHRS** (VectorNav)  

## Data Format  

The dataset is provided in CSV format, containing:  
- **Timestamp**  
- **Accelerometer Data** (X, Y, Z) [m/s²]  
- **Gyroscope Data** (X, Y, Z) [°/s]  
- **Magnetometer Data** (X, Y, Z) [µT]   

## Usage  

The dataset can be used for various applications, including:  
- Sensor fusion and calibration  
- Machine learning for motion tracking  
- Inertial navigation system (INS) research  

## License  

This dataset is available under the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/), allowing for free use with proper attribution.  

## Citation  

If you use this dataset in your research, please cite it as follows:  

