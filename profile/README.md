## Motion RL research: Optimized Real-Time Motion-Informed Planning

This organization hosts the complete, end-to-end intelligent agent pipeline for autonomous vehicle decision-making, focusing on research driven by the **Waymo Open Motion Dataset (WOMD)**.

We specialize in solving the critical challenges of **low-latency prediction** and **safety-critical planning** in highly interactive driving scenarios.

---

### The Core Problem Solved

This project creates a robust, two-stage solution to the core AV problem: converting slow, complex predictions into fast, safe actions.

| Module | Focus | Output | Technical Challenge Solved |
| :--- | :--- | :--- | :--- |
| **ORMF-3D** | **High-Performance Prediction** | Optimized **TensorRT** Engine | Solves the **Latency Problem** ($\mathbf{\text{sub-}20 \text{ ms}}$ inference speed). |
| **SCPF-RL** | **Safety Planning via DRL** | Safety-Optimized **PPO/SAC Policy** | Solves the **Interaction Problem** (Reduces failure rate in long-tail scenarios). |

---

### Technologies Stack

| Category | Key Technologies |
| :--- | :--- |
| **Core CV/Prediction** | **WOMD**, **PyTorch Geometric (GNN)** |
| **Inference Optimization** | **NVIDIA TensorRT (INT8/FP16)**, **FastAPI**, **Docker** |
| **Planning & Control** | **Stable-Baselines3 (PPO/SAC)**, **Gymnasium**, **Kinematic Bicycle Model** |
| **MLOps & Reproducibility** | **MLflow**, **Hydra**, **GitHub Actions** |

---

### Repositories

Browse the repositories below to explore the code, optimization details, and DRL training logic.

| Repository | Focus | Status |
| :--- | :--- | :--- |
| **[ormf-3d-forecasting]** | **Prediction Engine:** Focuses on model training, **TensorRT optimization**, and the production-ready **FastAPI** service for real-time trajectory output. | In Development |
| **[scpf-rl-planning]** | **Planning Agent:** Hosts the custom **Gymnasium Environment** and the **BC $\rightarrow$ PPO/SAC** workflow for fine-tuning the safety policy. | Planned |

### Evaluation Metrics (Safety First)

The success of the final policy is measured quantitatively over 500 closed-loop rollouts, focusing on:

* **Collision Rate** and **Time-to-Collision (TTC) Minimum**
* **Trajectory Smoothness (Jerk)**
* **Mean Distance to Lane Center**

---

### Contribution & Contact

This project is built for educational and portfolio purposes. Feel free to contact the owner for detailed discussions on the architecture or methodology.
