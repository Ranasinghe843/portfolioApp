# Robot Cello – Robotics Lead
**Senior Design | Purdue University Vertically Integrated Projects (VIP)**

### My Core Contribution
As the Robotics lead, I was responsible for building the functional foundation of the project. I developed the entire software-to-hardware pipeline, from the virtual simulation environment to the real-time kinematic controller for the **UR5e robotic arm**. My work enabled the team to transition from raw motion capture data to precise robotic movement.

---

### Simulation & Environment Design
I utilized **ROS2** and **Gazebo** to architect a high-fidelity digital twin of our laboratory environment.
* **Lab Mirroring:** Fully configured the simulation to accurately mirror the physical lab setup, including the UR5e arm, the cello, and custom mounting hardware.
* **Visualization:** Integrated **RVIZ** for real-time visualization and control of the arm’s manipulation.
* **Foundation for AI:** This simulation served as the primary training environment for the team's reinforcement learning models.

![Simulation Mirroring Setup](assets/images/ur5e.png)
---

### Kinematics & Control Pipeline
To achieve human-like bowing dexterity, I developed the logic required for precise joint manipulation.
* **Inverse Kinematics:** Wrote a custom script to convert 3D Cartesian coordinates into specific robot joint angles.
* **ROS2 Controller:** Created a controller that publishes joint angles at **0.002s intervals**, ensuring smooth, continuous pathways required for musical performance.
* **Accuracy Calibration:** Implemented scripts that take initial arm positions and calibration data to ensure the accuracy of the paths taken during the bowing motion.

---

### Data Processing & Engineering
I bridged the gap between human artistry and robotic execution by processing complex motion data.
* **MoCap Extraction:** Developed a pipeline to convert **FBX** motion capture files into **CSV** format, extracting position and orientation values for each marker.
* **Dataset Preparation:** Transformed these CSV files into joint-angle datasets ready for the training of behavioral cloning and learning models.

![Motion Capture Data](assets/images/mocap.png)

---

### Deliverables & Documentation
I ensured the project was reproducible and professionally documented for future research.
* **GitHub Repositories:** Delivered three distinct repositories containing the simulation code, the ROS2 controller, and the motion capture conversion scripts.
* **Technical Writing:** Authored detailed **README** files and a comprehensive senior design presentation outlining every design decision and the code logic.
* **Safety Integration:** Implemented boundary constraints within the control algorithms to ensure the safety of the human cellist and the instrument during collaborative performances.

> ****