# Hi, I'm Xingnan Zhou

**PhD Candidate in Transportation Engineering @ Concordia University, Montreal**

I build models that help autonomous vehicles predict trajectories and make safer decisions — from single-intersection forecasting to city-scale traffic simulation.

## Waymo E2E Driving Challenge

**[Ranked #15](https://waymo.com/open/challenges/e2e-driving/results/b34f2412-5a6e/1772305880072000/)** on the [Waymo Open Dataset End-to-End Driving Challenge](https://waymo.com/open/challenges/e2e-driving/) — trained on a single RTX 4090, Stage 1 pre-training only, no reinforcement learning yet.

| | |
|---|---|
| **Method** | [CTL-Drive](https://github.com/Jynxzzz/CTL-Drive) — Qwen3-VL-4B + QLoRA, CoVLA pre-training, intent conditioning, turn-aware fallback |
| **Training** | 795K frames (WOD-E2E + CoVLA), single RTX 4090 for Stage 1 |
| **Compute** | Scaling to [Google TPU Research Cloud](https://sites.research.google/trc/about/) — 288 TPU chips (v4-32, v5e-64, v6e-64), ~152 PFLOPS |
| **Next** | Stage 1b fine-tuning + GRPO reinforcement learning on TPU pods |
| **Details** | [Project page](https://obsicat.com/poutine-e2e.html) · [Leaderboard](https://waymo.com/open/challenges/e2e-driving/results/b34f2412-5a6e/1772305880072000/) |

## Research

My work spans **trajectory prediction**, **attention-based safety analysis**, **3D perception**, and **network-level traffic simulation**, primarily on the [Waymo Open Motion Dataset](https://waymo.com/open/) (89K+ intersection scenarios).

**Key contributions:**
- **Lane graph conditioning** — architecture-agnostic module that injects local lane topology into prediction models, achieving +26.7% minADE improvement on 89K Waymo scenarios
- **Training data geographic audit** — mapped 70K+ Waymo scenarios onto OpenStreetMap via topology fingerprinting (90% top-1 accuracy) to reveal what intersection types the dataset covers and where geographic blind spots exist
- **Attention safety analysis** — Transformer attention visualization revealing 63% higher miss rates for cyclists than vehicles — a critical safety blind spot, validated through counterfactual analysis
- **Dual-camera LiDAR fusion** — symmetric late fusion improving mAP by +4.4%, statistically validated across 10 seeds in CARLA simulation

## Featured Projects

| Project | Description | Highlights |
|---------|-------------|------------|
| [CTL-Drive](https://github.com/Jynxzzz/CTL-Drive) | VLM-based end-to-end driving on Waymo Challenge | **#15 leaderboard**, Google TPU Research Cloud |
| [Lane Graph Conditioning](https://github.com/Jynxzzz/lane-graph-conditioning) | Waterflow BFS extracts local lane graphs, cross-attention fuses topology into any predictor | +26.7% minADE, +43% miss rate ↓ on 89K Waymo scenes |
| [Network Dreamer](https://github.com/Jynxzzz/network-dreamer) | Maps Waymo scenarios onto OpenStreetMap to audit dataset geographic coverage and identify underrepresented intersection types | 90% top-1 accuracy, 70K scenarios, 17K routes |
| [Spatial Attention Viz](https://github.com/Jynxzzz/spatial-attention-viz) | Counterfactual analysis of Transformer attention maps in bird's-eye-view | 63% higher cyclist miss rate, tunnel vision failure mode |
| [Dual-Camera LiDAR Fusion](https://github.com/Jynxzzz/dual-camera-lidar-fusion) | Symmetric drone + dashboard camera late fusion for occluded 3D detection | +4.4% mAP (PointPillar), −13% false positives |
| [Turn-Aware LSTM](https://github.com/Jynxzzz/Turn-Aware-LSTM_SUPP) | Encoder-decoder with one-hot turn labels for intersection trajectory forecasting | 15–20% FDE ↓ on turning maneuvers |

## Tech Stack

**Research & ML:** Python, PyTorch, JAX, Waymo Open Dataset, CARLA, CUDA, Transformers, LSTM, GNN, YOLOv8, PointPillars

**Engineering:** TypeScript, Next.js, React, Three.js, Node.js, PostgreSQL, Docker, Vercel

**Tools:** Linux, Git, Neovim, Blender

*Published: [Turn-Aware LSTM for Vehicle Trajectory Forecasting](https://obsicat.com/turn-aware-lstm.html) (Advances in Transportation Studies, 2025) · See [obsicat.com](https://obsicat.com) for all projects and papers.*

## Links

[![Website](https://img.shields.io/badge/obsicat.com-Portfolio-1a2940?style=flat-square)](https://obsicat.com)
[![NudiLab](https://img.shields.io/badge/NudiLab-nudilab.art-d98c70?style=flat-square)](https://nudilab.art)
[![Email](https://img.shields.io/badge/Email-zhouxingnan2016@gmail.com-4ECDC4?style=flat-square)](mailto:zhouxingnan2016@gmail.com)
