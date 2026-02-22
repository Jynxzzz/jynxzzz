# Hi, I'm Xingnan Zhou

**PhD Candidate in Transportation Engineering @ Concordia University, Montreal**

I build models that help autonomous vehicles predict trajectories and make safer decisions — from single-intersection forecasting to city-scale traffic simulation.

## Research

My work spans **trajectory prediction**, **attention-based safety analysis**, **3D perception**, **network-level traffic simulation**, and **VLM-based end-to-end driving**, primarily on the [Waymo Open Motion Dataset](https://waymo.com/open/) (89K+ intersection scenarios).

**Key contributions:**
- **VLM end-to-end driving** — single-GPU reproduction of [Poutine](https://arxiv.org/abs/2502.01637) Stage 1 (VLT pre-training) on RTX 4090: built full training pipeline with Qwen3-VL-4B + QLoRA on 399K Waymo+CoVLA frames, with intersection-type-stratified evaluation
- **Lane graph conditioning** — architecture-agnostic module that injects local lane topology into prediction models, achieving +26.7% minADE improvement on 89K Waymo scenarios
- **GPS-free localization** — matching 70K+ driving scenarios to OpenStreetMap road networks with 90% top-1 accuracy via star-pattern topology fingerprinting
- **Attention safety analysis** — Transformer attention visualization revealing 63% higher miss rates for cyclists than vehicles — a critical safety blind spot, validated through counterfactual analysis
- **Dual-camera LiDAR fusion** — symmetric late fusion improving mAP by +4.4%, statistically validated across 10 seeds in CARLA simulation

## Publications

| Paper | Venue | Status |
|-------|-------|--------|
| [Turn-Aware LSTM for Vehicle Trajectory Forecasting](https://obsicat.com/turn-aware-lstm.html) | Advances in Transportation Studies | **Published 2025** |
| [Local Lane Graph Conditioning for Trajectory Prediction](https://obsicat.com/lane-conditioning.html) | — | In Preparation |
| [Discovering Safety Blind Spots Through Spatial Attention Visualization](https://obsicat.com/attention-visualization.html) | — | In Preparation |
| [Network Dreamer: Bridging Scenario-Level and Network-Level Simulation](https://obsicat.com/waygraph.html) | — | In Preparation |
| [Dual-Camera LiDAR Fusion for Occlusion-Robust 3D Detection](https://obsicat.com/bev-lidar-fusion.html) | — | In Preparation |
| [Reproducing Poutine: Single-GPU VLM E2E Driving Pipeline](https://obsicat.com/poutine-e2e.html) | — | Ongoing |

## Featured Projects

| Project | Description | Highlights |
|---------|-------------|------------|
| [Lane Graph Conditioning](https://github.com/Jynxzzz/lane-graph-conditioning) | Waterflow BFS extracts local lane graphs, cross-attention fuses topology into any predictor | +26.7% minADE, +43% miss rate ↓ on 89K Waymo scenes |
| [Network Dreamer](https://github.com/Jynxzzz/network-dreamer) | GPS-free localization framework placing Waymo scenarios onto OpenStreetMap road networks | 90% top-1 accuracy, 70K scenarios, 17K matched routes |
| [Spatial Attention Viz](https://github.com/Jynxzzz/spatial-attention-viz) | Counterfactual analysis of Transformer attention maps in bird's-eye-view | 63% higher cyclist miss rate, tunnel vision failure mode |
| [Dual-Camera LiDAR Fusion](https://github.com/Jynxzzz/dual-camera-lidar-fusion) | Symmetric drone + dashboard camera late fusion for occluded 3D detection | +4.4% mAP (PointPillar), −13% false positives |
| [Turn-Aware LSTM](https://github.com/Jynxzzz/Turn-Aware-LSTM_SUPP) | Encoder-decoder with one-hot turn labels for intersection trajectory forecasting | 15–20% FDE ↓ on turning maneuvers |
| [Reproducing Poutine](https://obsicat.com/poutine-e2e.html) | Single-GPU reproduction of [Poutine](https://arxiv.org/abs/2502.01637) Stage 1: full VLT pipeline on RTX 4090 | 399K frames, QLoRA fine-tuning, GRPO next |

## Tech Stack

**Research & ML:** Python, PyTorch, JAX, Waymo Open Dataset, CARLA, CUDA, Transformers, LSTM, GNN, YOLOv8, PointPillars

**Engineering:** TypeScript, Next.js, React, Three.js, Node.js, PostgreSQL, Docker, Vercel

**Tools:** Linux, Git, Neovim, Blender

## Links

[![Website](https://img.shields.io/badge/obsicat.com-Portfolio-1a2940?style=flat-square)](https://obsicat.com)
[![NudiLab](https://img.shields.io/badge/NudiLab-nudilab.art-d98c70?style=flat-square)](https://nudilab.art)
[![Email](https://img.shields.io/badge/Email-zhouxingnan2016@gmail.com-4ECDC4?style=flat-square)](mailto:zhouxingnan2016@gmail.com)
