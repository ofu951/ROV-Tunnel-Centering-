# Tunnel Averaging Algorithm for 3D Mapping

This project focuses on real-time processing of sonar data using a tunnel averaging algorithm. The collected binary data is first converted into floating-point numbers, and the average (center) point is calculated. These points are then used—together with data fusion from a Cable Counter, DVL (Doppler Velocity Log), and IMU (Inertial Measurement Unit)—to assist in constructing a 3D map.

## 🔧 How It Works

1. **Data Conversion:** Sonar data in binary format is converted to floating-point numbers.
2. **Center Point Calculation:** The algorithm calculates the average position using the last 10 data points.
3. **Real-time Visualization:** Displays the movement of the center point in either 2D or 3D.
4. **Sensor Fusion:** Combines Cable Counter, DVL, and IMU data for enhanced accuracy and 3D reconstruction.

## 📊 Sample Output

The image below shows the last 10 detected center points and their trajectory. It also displays statistics such as the total distance covered and the area mapped:

![Tunnel Averaging Visualization](image1.png)

> 📝 *Example visualization of real-time sonar data processing and movement tracking.*

## 📁 Project Status

This is the initial phase of a sonar data processing pipeline, aimed at assisting underwater 3D mapping and navigation systems.

## 🛠️ Technologies Used

- Python
- Matplotlib (for visualization)
- NumPy
- Serial communication (for binary data input)
- Sensor integration (Cable Counter, DVL, IMU)

## 🚀 Future Work

- 3D point cloud generation from fused sensor data
- Integration with SLAM frameworks
- Export to standard map formats (e.g., PCD, OBJ)

