# Paper reading notes


---

## Hot topics: drone / UAS development (research with commercial and defence relevance)

Curated list of **titles plus short pointers** you can use to locate PDFs in Scholar, the publisher, or the arXiv. Skews toward perception, control, swarms, GNSS-denied operation, and detection—areas that feed both industry products and military systems. You can turn each into a proper note file later.

- **Autonomous Drone Racing: A Survey** — Survey of agile, high-speed flight stacks (planning, perception, learning); the same control and latency challenges matter for small tactical or inspection platforms.

- **Champion-level drone racing using deep reinforcement learning** (Kaufmann et al., *Nature* 2023) — DRL that reaches human-champion performance in real-world racing; case study in learned policies under tight dynamics and sensor constraints.

- **Toward Autonomous UAV Swarm Navigation: A Review of Trajectory Design Paradigms** — Unifies classical, distributed, and learning-oriented trajectory design for many-UAV systems; base literature for swarming in logistics, agriculture, and cooperative missions.

- **UAV swarms: research, challenges, and future directions** — Broad 2020s review of swarm communication, task allocation, and coordination; good map of the research landscape before you dive into a subtopic.

- **Decentralized Control of Quadrotor Swarms with End-to-end Deep Reinforcement Learning** — End-to-end MARL for multi-quadrotor teams without a central policy; relevant to scalable autonomous formations.

- **RAPTOR: A Foundation Policy for Quadrotor Control** — “Foundation-style” single policy that generalises across different quadrotor dynamics; points toward standardised control stacks and faster integration on new airframes (R&D and systems houses).

- **Deep Reinforcement Learning for Robotics: A Survey of Real-World Successes** — Not drone-only, but has a strong quadrotor / locomotion thread; use it to see which RL ideas actually ship beyond simulation.

- **Control of UAV quadrotor using reinforcement learning and robust controller** (IET, 2023) — Hybrid RL + robust control for disturbances; useful when you need both adaptability and safety-case arguments (dual-use and certification-minded work).

- **GPS-Denied LiDAR-Based SLAM—A Survey** — LiDAR SLAM in denied-GNSS settings; directly relevant to military/navigation-denied scenarios and to high-end commercial mapping in GPS-challenged sites.

- **Survey on UAV Navigation in GPS Denied Environments** — Older umbrella survey on VIO, VO, and SLAM for UAS when satellite positioning is untrusted; good entry to vision-centric navigation for jamming/spoofing contexts.

- **A Survey of UAVs Detection: From Single UAV to Swarm** — Surveys detection/tracking of one and many UAS (RF, radar, vision, etc.); core science for counter-UAS, airspace monitoring, and base protection.

- **A Survey on Detection, Classification, and Tracking of UAVs Using Radar and Communications Systems** — Puts radar and comms/RF sides of the same problem in one frame; good for C-UAS sensor fusion and air-defence R&D.

- **A Comprehensive Survey of Unmanned Aerial Vehicles Detection and Classification Using Machine Learning Approach: Challenges, Solutions, and Future Directions** — ML/DL across modalities for detection and class labels; useful if your interest is data-driven C-UAS and airport perimeter systems.

*Tip:* In Google Scholar, paste the full title in quotes; if a title has changed slightly between preprint and journal, try the first six words and the lead author’s name.
