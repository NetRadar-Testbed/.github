# NetRadar

**An open-source networked mmWave radar testbed.** Several radar nodes (TI AWR2243 +
NVIDIA Jetson) capture on a shared, clock-synchronized hardware trigger and stream
detections to a fusion center that self-calibrates the network and fuses every
node's targets into one view.

<p align="center">
  <img src="netradar-testbed.jpg" width="820" alt="Four NetRadar radar nodes on tripods in a lab, with close-ups of one node's Jetson Orin Nano, DCA1000EVM capture card and AWR2243BOOST radar"><br>
  <em>A four-node NetRadar testbed. Each node: NVIDIA Jetson Orin Nano (compute + Wi-Fi), TI DCA1000EVM (ADC data capture), TI AWR2243BOOST (mmWave radar).</em>
</p>

<p align="center">
  <img src="self-calibration-demo.gif" width="640" alt="Animation: first each radar's tracks in its own coordinates, then the three radars' estimated positions and orientations with the same people aligned across radars"><br>
  <em>Self-calibration in action on a three-radar outdoor deployment (at UC Santa Barbara): first each radar's tracks in its own coordinates, then the estimated radar positions and orientations with the same people aligned across all three radars.</em>
</p>

Build your own testbed, on your own private network:

| Repository | |
| :--- | :--- |
| [**NetRadar-Node**](https://github.com/NetRadar-Testbed/NetRadar-Node) | Radar node software: real-time pipeline, trigger, installer |
| [**NetRadar-FusionCenter**](https://github.com/NetRadar-Testbed/NetRadar-FusionCenter) | Fusion center: MQTT broker, time sync, self-calibration, dashboard, database |
| [**Documentation**](https://netradar-testbed.github.io) | Step-by-step setup from scratch |

**Citing.** If you use NetRadar, or a testbed built with it, in published work, please
cite our papers and state that your testbed was built with NetRadar — see
[Citing NetRadar](https://netradar-testbed.github.io/citing/).

Developed as part of the **Chirp Capstone Project 2025–2026, University of California,
Santa Barbara.** Authors: William Ni, Oviya Seeniraj, Andrey Otvagin, Vihan Jayaraman,
Jason Wang, Anirban Banik. Mentor: Anirban Banik. Advising professors: Upamanyu Madhow,
Yogananda Isukapalli. Licensed under Apache-2.0.
