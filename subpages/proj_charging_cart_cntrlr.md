---
layout: default
---

# Mk. VIII Charging Cart Controller PCB
_January-February, 2026_

<img src="..\assets\img\charging_cart_controller_rendering.png" alt="BSPD PCB rendered on KiCAD" width="45%" centering=true>
<img src="..\assets\img\charging_cart_controller_traces.png" alt="BSPD PCB Traces rendered on KiCAD" width="45%" centering=true>

**Learnings:**
- Leadership
- People Administration
- PCB Design

**Project Summary:** This project was done while I was in the Co-Electrical Subsystem Lead position. This was originally a member's project that was heavily intervened in. I first let the member try to manage his time to get the project done while my partner (the other Co-Electrical Subsystem Lead, Jacob Likins) scaffolded the deadlines as much as possible. We walked through how the design was going to be and some theory like signals of similar speed should go near each other. In the end, we had to take over the project and design the PCB ourselves to get it done by the deadline to stay on track.

This was very much an exercise for people management for both of us as this situation would have hurt us a lot should we had not intervened. Thankfully, the problem was resolved and the PCB design was completed on time by myself.

As for the PCB design, we were working with a smaller size constraint in which we needed to reduce the overall footprint of the board. To accomplish this, we settled for a design in which everything was orientated based on the pin it would use from the microcontroller, avoiding trace cross overs. While it is not necessary to avoid cross overs since these signals are slow (less than 1 MHz), I thought that it was best practice and therefore I implemented it. The placement of the connectors were done in such a way where it would be easy to connect and disconnect the connectors when needed. The rectangular connector on the side was for an LCD display where the connector would serve both a physical and a electrical purpose. Physical to actually hold the display and electrical to pass the signals.