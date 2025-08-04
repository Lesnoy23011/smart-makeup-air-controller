# Smart Makeup Air Controller for Airtight Homes

An open-source ESPHome-based controller that provides **automated fresh air intake** when negative pressure is detected in airtight or passive homes. Built using the **LILYGO T-Relay ESP32 board**, this system monitors the use of exhaust appliances (kitchen hood, bathroom fan, dryer) and intelligently activates a **makeup air fan** to maintain pressure equilibrium.

---

## 🏠 Why This Project Matters

In highly sealed, energy-efficient homes, exhaust systems can create **negative air pressure**, leading to:
- Doors becoming difficult to open when appliances like kitchen hoods are active
- Reduced HVAC efficiency and backdraft risks
- Poor indoor air quality due to lack of fresh air replenishment

This project solves that by detecting when venting occurs and responding with the proper amount of filtered intake air.

---

## ✅ Key Features

- ESP32-based smart relay controller
- Integrates with **Home Assistant** via ESPHome
- **Real-time monitoring** of exhaust appliance usage
- Controls a **variable-speed makeup air fan**
- Uses **current sensors** to measure hood fan usage and adjust intake accordingly
- Designed for easy retrofit and expansion

---

## ⚙️ Core Components

- LILYGO T-Relay ESP32
- ESPHome firmware
- Current transformer or smart switch with power monitoring (e.g., Shelly EM, CT clamp)
- Inline intake fan with speed control
- Filtration system (optional)
- Home Assistant for sensor aggregation and automation

---

## 🛠 How It Works

1. A power-monitoring sensor detects current draw from exhaust appliances.
2. If current exceeds threshold, a relay or fan controller activates the makeup air intake.
3. Fan speed is modulated to match exhaust appliance power level.
4. All logic and adjustments are managed through **Home Assistant automations**.

---

## 💡 Future Features

- Pressure sensor integration
- CO₂ monitoring to trigger fresh air independently
- External weather-aware intake behavior

---

## 📜 License

MIT License (to be added)

---

*Built and maintained by Maksim Tsarenko • [LinkedIn](https://www.linkedin.com/in/maksim-tsarenko/)*
