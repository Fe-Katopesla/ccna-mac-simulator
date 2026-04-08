# 🖧 CCNA L2 Switch MAC Simulator

![Project Preview](https://github.com/user-attachments/assets/e3bb4a5e-74c2-44f2-b0d7-ce26c14b2474)

[![Live Demo](https://img.shields.io/badge/Live-Demo-2ecc71?style=for-the-badge&logo=github)](https://fe-katopesla.github.io/ccna-mac-simulator/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)]()

This project is an interactive simulator of a Local Area Network (LAN) topology focused on the behavior of a **Layer 2 Switch**. It was developed as a practical study tool for the **Cisco CCNA (200-125)** certification, visually illustrating how a switch builds its MAC Address Table and makes frame forwarding decisions.

---

## Project Objective

The main goal of this simulator is to practically demonstrate the three fundamental concepts of the Data Link Layer:
1. **Address Learning:** How the switch learns the source MAC address and the incoming port.
2. **Forward/Filter Decisions:** How the switch uses the MAC Table to forward a frame via Unicast.
3. **Loop Avoidance / Flooding:** How the switch handles frames with an unknown destination (Unknown Unicast).

---

## Features

* **Visual Traffic Simulation:** CSS animations showing the frame's journey from the source PC to the Switch, and from the Switch to the destination.
* **Dynamic MAC Table:** The table updates in real-time as soon as the Switch "learns" a new MAC address based on incoming traffic.
* **Flooding Logic:** If the destination PC is not yet in the MAC Table, the simulator demonstrates *Flooding*, sending the frame out all active ports (except the source).
* **Unicast Logic:** If the destination MAC is already known, the Switch sends the frame directly to the correct port.
* **Event Logs Console:** An integrated terminal narrating the Switch's cognitive process step-by-step ("Learning MAC", "Unknown Destination", "Forwarding Unicast").
* **Table Clear:** A button to reset the MAC Table, simulating purging due to inactivity (*Aging Timer*) or manual clearing by the network administrator.

---

## How to Run the Project

Since the project was built using only native front-end technologies (Vanilla JS), there is no need to install libraries, dependencies, or complex servers (Node, NPM, etc.).

### Option 1: Via GitHub Pages (Recommended)
Access the hosted version directly via the link:
**[Access the Online Simulator](https://fe-katopesla.github.io/ccna-mac-simulator/)**

### Option 2: Locally on your machine
1. Clone this repository:
   ```
   git clone [https://github.com/fe-katopesla/ccna-mac-simulator.git](https://github.com/fe-katopesla/ccna-mac-simulator.git)
  ``

2. Navigate to the project folder:
   ```bash
   cd ccna-mac-simulator
 ``
 ## Applied Networking Concepts

By using this simulator, you are validating the following topics covered in CCNA study guides:

* **OSI Layer:** Layer 2 (Data Link).
* **Component:** Ethernet Switch.
* **Memory:** CAM (Content Addressable Memory) Table.
* **Core Behavior:** Switches learn by observing the **Source MAC** and forward by observing the **Destination MAC**.

---

## Technologies Used

* **HTML5:** Semantic structuring of the topology and controls.
* **CSS3:** Responsive styling, Flexbox layout, and state transition animations (`transition` and DOM manipulation).
* **JavaScript (Vanilla):** MAC Table state logic, timing control (`Promises` and `setTimeout`), and dynamic event injection into the DOM.

 Applied Networking Concepts

By using this simulator, you are validating the following topics covered in CCNA study guides:

    OSI Layer: Layer 2 (Data Link).

    Component: Ethernet Switch.

    Memory: CAM (Content Addressable Memory) Table.

    Core Behavior: Switches learn by observing the Source MAC and forward by observing the Destination MAC.

 Technologies Used

    HTML5: Semantic structuring of the topology and controls.

    CSS3: Responsive styling, Flexbox layout, and state transition animations (transition and DOM manipulation).

    JavaScript (Vanilla): MAC Table state logic, timing control (Promises and setTimeout), and dynamic event injection into the DOM.
   
   Double-click the index.html file to open it in your favorite web browser (Chrome, Firefox, Edge, Safari).
   
   ```bash
   git clone [https://github.com/fe-katopesla/ccna-mac-simulator.git](https://github.com/fe-katopesla/ccna-mac-simulator.git)
