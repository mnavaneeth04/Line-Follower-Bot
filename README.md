# 🤖 Arduino Line Follower Robot

This repository contains the code and circuit setup for a simple **line follower robot** using an **Arduino Uno**, **IR sensors**, and an **L293D motor driver**. The robot is designed to follow a black line on a white surface by constantly reading input from two IR sensors and adjusting its motors accordingly.

---

## 📝 Description

The project uses two IR sensors to detect the color contrast between a black line and a white surface. Based on the sensor readings, the Arduino controls two DC motors via an **L293D motor driver** to follow the path.

### Working Logic:
- **Both sensors on white** → Move **forward**
- **Right sensor on black** → **Turn right**
- **Left sensor on black** → **Turn left**
- **Both sensors on black** → **Stop** (e.g., end of path or intersection)

The robot is coded using the **Arduino programming language (C/C++)** and is compatible with the **Arduino IDE**.

---

## 🧰 Hardware Requirements

- Arduino Uno (or compatible board)  
- L293D Motor Driver Module  
- DC Motors (x2)  
- IR Sensors (x2)  
- Wheels + Chassis  
- Power source (battery pack)  
- Jumper wires, breadboard (optional)

---

## ⚙️ Pin Configuration

| Component       | Arduino Pin |
|----------------|-------------|
| Right IR Sensor| D4          |
| Left IR Sensor | D2          |
| ENA (Motor A)  | D5          |
| IN1            | D7          |
| IN2            | D6          |
| IN3            | D10         |
| IN4            | D9          |
| ENB (Motor B)  | D11         |

---

## 🚀 Usage

1. Connect all hardware as per the wiring diagram.
2. Open the `.ino` file in **Arduino IDE**.
3. Upload the code to your Arduino board.
4. Place the robot on a track with a **black line on white surface**.
5. Power it on and watch it follow the line!

---

## 🛠️ Technologies Used

- Arduino Uno  
- Arduino IDE  
- Embedded C/C++  
- IR Sensor Logic  
- PWM Motor Control  

---

## 📈 Behavior Summary

| Sensor Reading (Left, Right) | Action        |
|------------------------------|---------------|
| White, White                 | Move Forward  |
| Black, White                 | Turn Right    |
| White, Black                 | Turn Left     |
| Black, Black                 | Stop          |

---

## 🔮 Future Enhancements

- Add PID control for smoother turns  
- Include a third center IR sensor for better stability  
- Integrate speed control based on curve detection  
- Add Bluetooth or Wi-Fi control for remote override  

---

## 🙌 Acknowledgements

- Open-source robotics tutorials  
- Arduino and sensor documentation  
- Community forums and contributors  
