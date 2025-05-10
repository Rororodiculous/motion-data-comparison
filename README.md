# Motion Data Comparison Tool

This web-based tool simulates the motion of a car under constant acceleration, providing two types of simulated sensor data:

- **Position data** with low-frequency noise (as from a GPS or rangefinder)
- **Acceleration data** with higher-frequency jitter (as from an onboard accelerometer)

It is designed for physics education, giving students the opportunity to explore how velocity can be derived from different types of data using numerical methods.

## Features
- Uses the equation:  
  **x(t) = x₀ + v₀ * t + 1/2 * a * t²**
- Randomized **true acceleration** between **0.5 and 1.5 m/s²**
- Randomized **initial velocity** between **0 and 2 m/s**
- Position data has <5% smooth random noise
- Acceleration data has up to ±10% jittery noise
- 25 time points sampled every 0.5 seconds
- Output is formatted as **CSV** for easy pasting into Excel or Google Sheets

## Format of Output
Simulated Motion Data
Velocity Comparison via Derivatives and Integrals
True Acceleration: 1.021 m/s²
Initial Velocity: 0.862 m/s

Time,Position,Acceleration

0.00,0.0000,1.0543

0.50,0.2781,0.9312

...


## How to Use
1. Visit the web page  
2. Click the **"Generate New Data Set"** button  
3. Copy and paste the output into a spreadsheet  
4. Use Excel to compute:  
   - Velocity by differentiating position  
   - Velocity by integrating acceleration  
   - Compare the results

## Pros and Cons of Each Sensor Type
- **Position Sensor (e.g., GPS)**  
  ✅ Smooth results  
  ❌ May miss rapid changes or be less accurate over short intervals

- **Accelerometer**  
  ✅ Captures rapid dynamics  
  ❌ Drift and noise accumulate when integrating

Students are encouraged to compare these methods and explore how sensor uncertainty impacts velocity estimates.

## Access the Tool
🔗 [Motion Data Comparison Webpage](https://yourusername.github.io/motion-data-comparison/)

> Replace `yourusername` with your GitHub username

## License
This project is open source and available under the MIT License.

---
*Developed for real-world physics education in motion analysis.*
