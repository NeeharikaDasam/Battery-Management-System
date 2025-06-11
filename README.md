## 🔋 **Battery Voltage Monitoring System using Arduino Uno**

### ✅ **Project Overview:**

This project is designed to monitor the **voltage levels of a battery pack** in real-time using an Arduino Uno. It utilizes analog voltage sensors to measure individual cell voltages and displays the readings on a 16x2 I2C LCD. The system helps in identifying under-voltage conditions and tracking the battery pack’s total voltage during charging or discharging.

---

### 🛠️ **Components Used:**

* Arduino Uno
* 16x2 LCD with I2C module
* Voltage sensor module (or voltage dividers)
* Current sensor (ACS712) *(optional)*
* DHT11 temperature sensor *(optional)*
* Relay module *(optional for protection/automation)*
* Wires, breadboard, power source (battery)

---

### ⚙️ **Key Features:**

* Real-time monitoring of **up to 4 individual battery cells**
* **Total and Pack voltage** calculation
* **LCD display output** with clean data visualization
* **Serial monitor logging** for debugging and logging
* Expandable to include **current and temperature monitoring**
* Optionally control load or charging via a **relay**

---

### 🔌 **Working Principle:**

* The analog pins of Arduino (A0 to A3) read voltages through a voltage divider or sensor.
* Each analog reading is converted to an actual voltage using a scaling factor.
* The code calculates total and pack voltage and displays it on the LCD.
* If integrated, the current sensor measures real-time current, and the DHT11 gives temperature and humidity data.
* The system can be used to trigger a relay in case of over/under-voltage.

---

### 📟 **Output Example (LCD):**

```
C1:3.68 C2:3.65
C3:3.70 C4:3.69
---
Total:14.72V
Pack: 14.81V
```

---

### 📈 **Applications:**

* Battery management systems (BMS)
* Electric vehicle battery diagnostics
* Solar battery monitoring
* Lab experiments for energy systems
