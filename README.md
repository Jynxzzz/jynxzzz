# Hi, I'm Xingnan Zhou

**PhD Candidate in Transportation Engineering @ Concordia University, Montreal**

I build models that help autonomous vehicles predict trajectories and make safer decisions — from single-intersection forecasting to city-scale traffic simulation.

## Research

My work spans **trajectory prediction**, **attention-based safety analysis**, **3D perception**, and **network-level traffic simulation**, primarily on the [Waymo Open Motion Dataset](https://waymo.com/open/) (89K+ intersection scenarios).

**Key contributions:**
- **Lane graph conditioning** — architecture-agnostic module that injects local lane topology into prediction models, achieving +27% minADE and +43% miss rate reduction
- **GPS-free localization** — matching 70K+ driving scenarios to OpenStreetMap road networks with 90% top-1 accuracy via star-pattern topology fingerprinting
- **Attention safety analysis** — revealing that Transformer models allocate 73% less attention to cyclists and 60% less to pedestrians, with counterfactual validation
- **Dual-camera LiDAR fusion** — symmetric late fusion reducing false positives by 13%, improving mAP by +4.4% on PointPillar in CARLA simulation

## Publications

| Paper | Venue | Status |
|-------|-------|--------|
| [Turn-Aware LSTM for Vehicle Trajectory Forecasting](https://obsicat.com/turn-aware-lstm.html) | Advances in Transportation Studies | **Published 2025** |
| [Local Lane Graph Conditioning for Trajectory Prediction](https://obsicat.com/lane-conditioning.html) | MDPI Sustainability | Preparing |
| [Discovering Safety Blind Spots Through Spatial Attention Visualization](https://obsicat.com/attention-visualization.html) | MDPI Sustainability | Preparing |
| [Network Dreamer: Bridging Scenario-Level and Network-Level Simulation](https://obsicat.com/waygraph.html) | MDPI Sustainability / IEEE ITSC | Preparing |
| [Dual-Camera LiDAR Fusion for Occlusion-Robust 3D Detection](https://obsicat.com/bev-lidar-fusion.html) | MDPI Sustainability | Preparing |

## Featured Projects

| Project | Description | Highlights |
|---------|-------------|------------|
| [Lane Graph Conditioning](https://github.com/Jynxzzz/lane-graph-conditioning) | Waterflow BFS extracts local lane graphs, cross-attention fuses topology into any predictor | +27% minADE, +43% miss rate ↓ on 89K Waymo scenes |
| [Network Dreamer](https://github.com/Jynxzzz/network-dreamer) | GPS-free localization framework placing Waymo scenarios onto OpenStreetMap road networks | 90% top-1 accuracy, 70K scenarios, 17K matched routes |
| [Spatial Attention Viz](https://github.com/Jynxzzz/spatial-attention-viz) | Counterfactual analysis of Transformer attention maps in bird's-eye-view | 73% cyclist attention deficit, tunnel vision failure mode |
| [Dual-Camera LiDAR Fusion](https://github.com/Jynxzzz/dual-camera-lidar-fusion) | Symmetric drone + dashboard camera late fusion for occluded 3D detection | +4.4% mAP (PointPillar), −13% false positives |
| [Turn-Aware LSTM](https://github.com/Jynxzzz/Turn-Aware-LSTM_SUPP) | Encoder-decoder with one-hot turn labels for intersection trajectory forecasting | 15–20% FDE ↓ on turning maneuvers |

## Tech Stack

**Research & ML:** Python, PyTorch, JAX, Waymo Open Dataset, CARLA, CUDA, Transformers, LSTM, GNN, YOLOv8, PointPillars

**Engineering:** TypeScript, Next.js, React, Three.js, Node.js, PostgreSQL, Docker, Vercel

**Tools:** Linux, Git, Neovim, Blender

## Links

[![Website](https://img.shields.io/badge/obsicat.com-Portfolio-1a2940?style=flat-square)](https://obsicat.com)
[![NudiLab](https://img.shields.io/badge/NudiLab-nudilab.art-d98c70?style=flat-square)](https://nudilab.art)
[![Email](https://img.shields.io/badge/Email-zhouxingnan2016@gmail.com-4ECDC4?style=flat-square)](mailto:zhouxingnan2016@gmail.com)
