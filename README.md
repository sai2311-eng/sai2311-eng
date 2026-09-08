## Sai Kiran

**Mechanical engineer. Master's student in Mechatronics and Cyber-Physical Systems, graduating 2027. Building a career in robotics.** Based in Germany.

Robotics is where my field stops being mechanical and starts being autonomous, and I'd rather own that whole span than half of it. Mechanics, electronics, control and software are one system, so I'm learning to build it as one: design a robot, print it, and teach it to navigate a room it has never seen.

---

### What I'm building

**A differential-drive mobile robot — designed, 3D-printed, and driven by ROS 2.**

The chassis, wheel hubs and motor mounts are my own designs, modelled in Fusion 360 and printed at home. The control side is split across two processors — the cyber-physical split my coursework is about, made concrete: a general-purpose Linux machine cannot hold a hard real-time deadline, so an **ESP32 running micro-ROS** owns the encoders, PWM and the PID velocity loop, and streams over WiFi to **ROS 2 Jazzy** running the navigation stack. Odometry first, then SLAM, then autonomy.

**ROS 2 Jazzy** — nodes, topics, services, parameters and launch files in `rclpy`, then the same concepts re-implemented in `rclcpp`. Simulation in Gazebo Harmonic where the hardware isn't ready, on the real drivetrain where it is.

A five-month plan runs from August to December 2026 and ships five projects rather than five certificates:

| | Project | Stack |
|---|---|---|
| 1 | Turtle Chase — multi-node pursuit with dynamic spawning | `rclpy` |
| 2 | Sensor filter node — real-time signal conditioning | `rclcpp` |
| 3 | The printed diff-drive robot — URDF, TF tree, closed-loop odometry | micro-ROS, ESP32 |
| 4 | Autonomous navigator — SLAM and Nav2 in an unmapped room | Nav2, slam_toolbox |
| 5 | Vision-guided delivery capstone | OpenCV, Nav2 |

Each gets its own repository. Progress is measured in things that move.

---

### Software projects

Not my profession — these are how I taught myself to build systems, and they're here as evidence that I can.

**[cached_csv_loader](https://github.com/BennyThadikaran/fast_csv_loader/pull/2)** — merged upstream, May 2026
Added mtime-aware in-memory caching to `fast_csv_loader`, so repeated loads of an unchanged file skip disk entirely and a stale read is impossible. 355 lines across 4 files, reviewed and merged by the maintainer.

**[आयुष — Sacred Lifespan Clock](https://sai2311-eng.github.io/ayush/)** — [source](https://github.com/sai2311-eng/ayush)
An offline-first PWA that counts your remaining heartbeats, framed by the four Ashrams of life. 12 Indian languages, 295 sourced quotes, installable to a home screen, works with zero network after first load. Click it — it runs.

**[Agnes — supply-chain intelligence](https://github.com/sai2311-eng/NIKOLA)** — TUM.ai × Spherecast hackathon, April 2026
Competed on Spherecast's challenge to give their "Agnes" AI supply-chain manager raw-material superpowers. Built supplier discovery across 11+ sources, live HS-code lookup with SQLite caching, compliance scoring against 8 international standards, and a substitution engine that finds functionally equivalent materials.

**[BillHound](https://github.com/sai2311-eng/billhound)** — autonomous bill auditor
An agent that reads every bill you receive and speaks only when something is wrong: off-contract rates, duplicated line items, totals that don't reconcile. Built on the Strands Agents SDK over Amazon Bedrock. The design goal was restraint.

---

### Tools

**Mechanical** — Fusion 360 · 3D printing (FDM) · design for manufacture
**Embedded & control** — ESP32 · micro-ROS · PID control · encoders, PWM, IMU
**Software** — Python · C++ · ROS 2 Jazzy · Linux · Git
**Simulation** — Gazebo Harmonic · RViz2 · URDF

---

*Open to working-student and thesis positions now, and to robotics engineering roles in Germany from 2027.*
