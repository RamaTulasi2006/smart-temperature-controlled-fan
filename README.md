# 🌡️ Smart Temperature Controlled Fan using Arduino

## 📌 Project Overview
This project is designed to automatically control the speed of a fan based on the surrounding temperature. It uses a temperature sensor to continuously monitor the environment and adjusts the fan speed using PWM (Pulse Width Modulation).

The main objective of this project is to improve energy efficiency and provide an automated cooling solution.

---

## 🛠️ Components Used
- Arduino Uno
- Temperature Sensor (LM35)
- DC Fan / Motor
- Transistor (for switching)
- Resistors
- Power Supply
- Connecting Wires

---

## ⚙️ Working Principle
1. The LM35 sensor reads the ambient temperature.
2. Arduino converts the analog signal into temperature (°C).
3. Based on temperature:
   - Low temperature → Fan OFF
   - Medium temperature → Fan runs at medium speed
   - High temperature → Fan runs at full speed
4. PWM signal controls the fan speed.

---

## 💻 Code Logic
- `analogRead()` → reads temperature sensor value  
- Conversion formula → converts to °C  
- `if-else` conditions → decide fan speed  
- `analogWrite()` → controls PWM (fan speed)

---

## 📊 Output Behavior
| Temperature Range | Fan Speed |
|------------------|----------|
| < 25°C           | OFF      |
| 25°C – 35°C      | Medium   |
| > 35°C           | High     |

---

## 🚀 Applications
- Smart Homes
- Automatic Cooling Systems
- Energy Efficient Devices
- Industrial Temperature Control

---

## 🔮 Future Improvements
- Add IoT (mobile app control)
- Display temperature on LCD
- Use advanced sensors for accuracy
- Voice control integration

---

## 📸 Circuit Diagram
![Circuit](images/circuit.png)

## 🔧 Hardware Setup
![Setup](images/setup.png)

## 📊 Output
![Output](images/output.png)


---

## 👨‍💻 Author
Rama Tulasi
