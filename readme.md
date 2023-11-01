# Intelligent Soil Monitoring and Plant Care System

## Overview
This project uses the ESP8266 as the primary controller, combined with the DHT22 sensor, Raspberry Pi, and additional hardware components, to create a smart soil monitoring system. The main objective is to monitor the soil's temperature, humidity, and voltage values in real-time to determine if plants require watering. When watering is needed, a buzzer alerts the user.
![introduction](https://github.com/QingyaoTang/Plant-Monitor/blob/main/WechatIMG1593.jpg)
## Key Features:
1. **Real-Time Monitoring**: The system constantly measures the temperature, humidity, and voltage values of the soil.
2. **Remote Access**: The ESP8266 Wi-Fi module facilitates internet connectivity, granting users remote access to monitor the plant environment.
3. **Data Storage & Analysis**: Uses Influx DB for data storage and Telegraf for data collection, aiding in real-time analytics.
4. **Web Interface**: Allows users to visually access soil data, ensuring informed decisions on plant care.
5. **Audible Alerts**: A buzzer alerts the user when the system detects that the soil temperature is too high or the humidity is too low.
6. **Time Synchronization**: An online time synchronization function ensures accurate system timekeeping.
![introduction](https://github.com/QingyaoTang/Plant-Monitor/blob/main/WechatIMG1610.jpg)
## Hardware Used:
- DHT22 Sensor
![DHT22](https://github.com/QingyaoTang/Plant-Monitor/blob/main/WechatIMG1594.jpg)
- Iron Nails
- Buzzer
- ESP8266
![ESP8266](https://github.com/QingyaoTang/Plant-Monitor/blob/main/WechatIMG1595.jpg)
- Raspberry Pi
![Raspberry Pi](https://github.com/QingyaoTang/Plant-Monitor/blob/main/WechatIMG1597.jpg)

## Software Used:
- MQTT
![MQTT](https://github.com/QingyaoTang/Plant-Monitor/blob/main/Screenshot%202023-11-01%20at%2010.36.17.png)
- Arduino IDE
![Arduino IDE](https://github.com/QingyaoTang/Plant-Monitor/blob/main/Screenshot%202023-11-01%20at%2011.01.14.png)
- GitHub
![github](https://github.com/QingyaoTang/Plant-Monitor/blob/main/Screenshot%202023-11-01%20at%2010.45.59.png)
- InfluxDB
![InfluxDB](https://github.com/QingyaoTang/Plant-Monitor/blob/main/Screenshot%202023-11-01%20at%2010.25.42.png)
- Telegraf

## Step 1: Hardware Assembly

1. Connect the DHT22 sensor to the ESP8266, ensuring the connections are correct.
2. Insert the DHT22 sensor into the soil of the plant using iron nails.
3. Connect the buzzer to the ESP8266 to enable it to produce alerts.
4. Connect the Raspberry Pi to the ESP8266 for internet connectivity.

## Step 2: Software Installation

1. Install the Arduino IDE and open the Arduino code for the project.
2. Configure the Wi-Fi settings in the Arduino code to ensure the ESP8266 connects to the internet correctly.
3. Install InfluxDB and Telegraf and ensure they are running properly.

## Step 3: GitHub Project

1. Access the GitHub repository: [github](https://github.com/QingyaoTang).
2. Clone the project to your local computer.
3. Follow the instructions in the README file to configure the GitHub repository.

## Step 4: System Start-Up

1. Start the ESP8266 and Raspberry Pi.
2. Monitor the system output to ensure sensor data is successfully uploaded to InfluxDB.
3. Access real-time data by using a web browser to visit the IP address of the Raspberry Pi.

## Step 5: Maintenance and Calibration

1. Regularly calibrate the sensors to ensure accuracy.
2. Maintain the system to ensure hardware is functioning correctly.
3. Address any issues or error messages.

## Limitations:
1. **Accuracy of Moisture Measurement**: The use of nails might result in inaccurate moisture readings due to various soil factors.
2. **Data Analysis & Decision Making**: Decisions on watering depend on various factors, requiring more advanced algorithms.
3. **Environmental Interference**: Conditions such as sunlight and temperature can interfere with sensor readings.
4. **Maintenance & Calibration**: Regular calibration is essential to ensure accurate sensor readings.

## Challenges & Solutions:
1. **Environmental Disturbance**:
   - **Challenge**: The DHT22 sensor is susceptible to environmental factors.
   - **Solution**: A protective shield for the DHT22 sensor can mitigate environmental interference.
2. **Data Accuracy**:
   - **Challenge**: Iron nails can be influenced by other metal ions in the soil.
   - **Solution**: Implementing a calibration procedure or using specialized soil moisture sensors can enhance accuracy.

By addressing these challenges, users can better ensure their plants receive the best care possible, optimizing plant health and growth.










