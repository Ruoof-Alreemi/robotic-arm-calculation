# robotic-arm-calculation
To determine the necessary torque for each motor in a robotic arm, follow these steps:  

---

## **1. Calculate the Required Torque for Each Joint**  

### **Given Data:**  
- **Total mass of the arm:** 1 kg  
- **Arm dimensions:**  
  - **Upper arm length:** 10 cm  
  - **Lower arm length:** 15 cm  
  - **Distance from joint to center of mass:** 4 cm  

### **Torque Formula:**  
The torque (\(\tau\)) is given by the equation:  

\[
\tau = r \times F
\]

where:  
- **\(\tau\)** = Torque (Newton-meter).  
- **\(r\)** = Lever arm distance (meters).  
- **\(F\)** = Force due to gravity (Newtons).  

### **Compute Force Due to Gravity:**  
Force (\(F\)) is calculated as:  

\[
F = m \times g
\]

where:  
- **\(m\)** = 1 kg (mass of the arm).  
- **\(g\)** = 9.81 m/s² (gravitational acceleration).  

\[
F = 1 \times 9.81 = 9.81 \text{ N}
\]

---

## **2. Compute Torque for Each Joint**  

### **Joint 1 (Upper Arm):**  
- **Lever arm distance (\(r\))** = 10 cm = 0.1 m  
- **Force (\(F\))** = 9.81 N  

\[
\tau_1 = 0.1 \times 9.81 = 0.981 \text{ Nm}
\]

### **Joint 2 (Lower Arm):**  
- **Lever arm distance (\(r\))** = 15 cm = 0.15 m  
- **Force (\(F\))** = 9.81 N  

\[
\tau_2 = 0.15 \times 9.81 = 1.4715 \text{ Nm}
\]

---

## **3. Choosing the Right Servo Motors**  

To ensure efficient performance, the selected motors should have torque ratings **exceeding** the required values:  

- **For Joint 1:** The motor should provide more than **0.981 Nm** (recommended range: **1-2 Nm**).  
- **For Joint 2:** The motor should provide more than **1.4715 Nm** (recommended range: **2-3 Nm**).  

By selecting motors with adequate torque, the robotic arm can function smoothly and handle additional loads if necessary.
