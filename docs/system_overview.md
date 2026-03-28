# System Overview

## High-Level Flow

1. Camera captures a frame  
2. AI detects plastic objects  
3. Position + size used to guide movement  
4. Robot navigates toward the target  
5. Ferrofluid interacts with plastic  
6. Magnetic drum assists recovery  
7. Plastic collected on the platform  

---

## Subsystems

### Vision System
- Camera + Fined tuned Computer Vision Model + OpenCV preprocessing (Saves compute time)
- Detection model (YOLOv8 Trained on Custome Hand Annotated Dataset)

### Control System
- Raspberry Pi → high-level decisions, run AI and convert predictions to signals
- ESP32 → Signal converting
- TB6612FNG → Motor control

### Mechanical System
- Floating chassis
- Drum + paddle propulsion

### Chemical System
- Custom ferrofluid formulation
