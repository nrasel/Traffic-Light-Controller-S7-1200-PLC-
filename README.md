# 🚦 Traffic Light Logic using Siemens S7-1200 PLC & TP700 HMI

## 📌 Project Overview
This project demonstrates a **traffic light control system** implemented using a **Siemens S7-1200 PLC (CPU 1212C DC/DC/DC)** and a **TP700 Comfort HMI panel**.  
The system simulates a real-world traffic junction where **North, West, and East directions** are controlled by a sequential traffic light program.

The goal of this project is to model the safe and efficient switching of traffic signals with a defined cycle of **green (15 sec)**, **yellow (5 sec)**, and **red** lights.

---

## 🛠 Hardware Used
- **PLC**: Siemens **S7-1200 CPU 1212C DC/DC/DC**  
- **HMI**: Siemens **TP700 Comfort Panel**  
- **Software**: TIA Portal (Step 7 + WinCC Comfort/Advanced)  

---

## 🔄 Traffic Light Sequence
The system follows a **3-step cycle**:

| Step | North | West | East |

| **1** | 🔴 Red | 🔴 Red | 🟢 Green (15s) → 🟡 Yellow (5s) |
| **2** | 🔴 Red | 🟢 Green (15s) → 🟡 Yellow (5s) | 🔴 Red |
| **3** | 🟢 Green (15s) → 🟡 Yellow (5s) | 🔴 Red | 🔴 Red |

- Each **green phase = 15 seconds**  
- Each **yellow phase = 5 seconds**  
- Red lights remain ON during other directions' green phases  

---

## 📊 Features
- Fully automated **traffic light cycle** using PLC logic  
- **Timers (TON)** used for signal duration handling  
- **Sequential switching** ensuring no conflicting green signals  
- **HMI TP700** provides real-time visualization of the junction with traffic lights animation  

---

## 🖥 HMI Design
- Graphical interface designed on **TP700 Comfort Panel**  
- Displays **traffic light states** (Red, Yellow, Green)  
- Allows operator to **monitor and simulate traffic flow**  

---

## 📂 Project Files
- **PLC Program**: Written in **LAD in TIA Portal**  
- **HMI Screens**: Designed in **WinCC Comfort**  

---

## 🚀 How to Run
    Clone the repository
            git clone https://github.com/nrasel/Traffic-Light-Controller-S7-1200-PLC-.git
            cd Traffic-Light-Controller-S7-1200-PLC
1. Open project in **TIA Portal**  
2. Download program to **S7-1200 CPU 1212C**  
3. Deploy HMI screens to **TP700 Comfort Panel**  
4. Observe traffic lights switching automatically based on logic

---

## 📷 Project View
![Traffic Light Interface](https://github.com/nrasel/Traffic-Light-Controller-S7-1200-PLC-/blob/94b85c9b68ba0877c091dba11bfa56e175933fa2/View%20Of%20the%20Project.PNG)


