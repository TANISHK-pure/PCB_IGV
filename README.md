# PCB_IGV
🚀 Custom IGV Motherboard – Gujcost Robofest 5.0

📋 Overview
A custom-designed 2-layer printed circuit board (PCB) engineered to serve as the central command and power distribution hub for an Intelligent Ground Vehicle (IGV). This board bridges high-performance 3.3V logic processing with rugged, high-current 5V robotics hardware.

🔌 Hardware Architecture & Tech StackMicrocontroller: Teensy 4.0 (ARM Cortex-M7)
EDA Software: EasyEDA
Logic Translation: ET5244 4-Channel Bi-Directional Logic Level Converters (3.3V - 5V)
PCB Specs: 2-Layer FR-4, 1.6mm thickness, 1 oz copper, HASL finish
Dimensions: 96.77 mm × 70.23 mm

🧠 Engineering Challenges Solved
1. Mixed-Voltage Signal Integrity
Interfacing a 3.3V microcontroller with 5V industrial optical encoders can cause signal degradation or hardware damage. I integrated an ET5244 logic level shifting circuit directly onto the board to safely step-up and step-down high-speed data signals in real-time.

2. High-Current Power Distribution (Trace Width Management)
To prevent board trace overheating under motor loads, I segmented the power rails. High-current lines (Main VBAT and 5V external inputs) were routed using 1.0mm to 1.5mm thick traces, while low-current sensor data and PWM logic were routed with precise 0.3mm traces.

3. EMI Noise Reduction
Heavy DC motors generate massive electromagnetic interference (EMI). I implemented comprehensive Top and Bottom Layer Ground Pours (copper flooding), eliminating "copper islands" through via-stitching and bottom-layer routing. This created a solid ground plane that absorbs noise and stabilizes logic signals.

4. Plug-and-Play Competition Readiness
Designed custom male/female header breakouts for front/rear motor drivers (PWM/DIR), cooling fans, and four independent optical encoders. This modular approach allows for instant hot-swapping of damaged external hardware during live competition scenarios.

🚦 Manufacturing Status
DRC Check: Cleared (0 Errors)

Fabrication: Gerber files generated and optimized for JLCPCB manufacturing standards.

🤝 Let's Connect
I am always open to discussing hardware architecture, custom PCB design, and embedded systems.

💼 LinkedIn: https://www.linkedin.com/in/tanishk-choudhary-215b95328/

📧 Email: ctanishk8@gmail.com
