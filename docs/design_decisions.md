# Design Decisions

## **Collection System:** Ferrofluid-Based Capture vs Mechanical Collection
Why ferrofluid instead of nets or filters:
- Enables selective interaction with non-polar plastics
- Avoids bulk water intake and clogging
- Reduces unintended capture of non-target materials

Tradeoffs:
- Requires strong containment strategy
- Performance may vary with plastics coated with something else

---

## **Collection System:** Permanent Magnets vs Electromagnets
Choice:
- Used permanent magnets

Reason:
- Lower power consumption
- Simpler integration
- Less failure points
- Continuous magnetic field without control systems

Tradeoffs:
- Less dynamic control compared to electromagnets

---

##  **Piloting:** Onboard AI vs Remote Processing
Choice:
- Onboard (Raspberry Pi)

Reason:
- Real-time response
- No reliance on external connection
- Enables autonomous operation

Tradeoffs:
- Limited computing power
- Required lots of optimization (TFLite, frame skipping, etc.)

---

##  **Movement:**  Paddles vs Thrusters/Propellers
Choice:
- Paddles

Reason:
- Faster iteration and testing
- Easier debugging

Tradeoffs:
- Poor containment
- Not suitable for real-world deployment yet
