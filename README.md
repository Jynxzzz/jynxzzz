# Hi, I'm Xingnan Zhou

**PhD Candidate in Transportation Engineering @ Concordia University, Montreal**

I study how autonomous vehicles predict trajectories and make safer decisions. I also build full-stack products — because research that can't ship is just a PDF.

## Research

My work focuses on **trajectory prediction** and **3D perception** for autonomous driving, primarily on the [Waymo Open Motion Dataset](https://waymo.com/open/) (89K+ scenarios).

**Key contributions:**
- **Lane graph conditioning** that improves trajectory prediction by +27% minADE — architecture-agnostic, works with both LSTM and Transformers
- **GPS-free localization** matching driving scenarios to OpenStreetMap with 90% top-1 accuracy using topology fingerprinting
- **Attention analysis** revealing that Transformer models allocate 60% less attention to vulnerable road users — a quantifiable safety blind spot
- **Dual-camera LiDAR fusion** improving occluded object detection by +11% mAP on CARLA

## Selected Publications

| Paper | Venue | Status |
|-------|-------|--------|
| [Turn-Aware LSTM for Vehicle Trajectory Forecasting](https://obsicat.com/turn-aware-lstm.html) | Advances in Transportation Studies | Published 2025 |
| [Local Lane Graph Conditioning for Trajectory Prediction](https://obsicat.com/lane-conditioning.html) | MDPI Sustainability | Under Review |
| [WayGraph: GPS-Free Localization onto OpenStreetMap](https://obsicat.com/waygraph.html) | MDPI Sustainability | Under Review |

## Featured Projects

### Autonomous Driving & Research
- **[WayGraph](https://github.com/Jynxzzz/waygraph)** — GPS-free localization of 89K Waymo scenarios onto OpenStreetMap via star-pattern topology fingerprinting
- **[Scenario Dreamer](https://github.com/Jynxzzz/scenario-dreamer-jynxzzz)** — Scenario generation and Transformer attention visualization on Waymo Open Motion Dataset
- **[Turn-Aware LSTM](https://github.com/Jynxzzz/Turn-Aware-LSTM_SUPP)** — Supplementary code for published trajectory prediction paper (15-20% FDE reduction at turns)

### Full-Stack Engineering
- **[NudiLab](https://nudilab.art)** — Production e-commerce platform for 3D-printed sculptural jewelry. Built with Next.js 16, React 19, Three.js, Stripe, and Supabase. Features interactive 3D product viewer with SLA print simulation, multi-material pricing, order tracking, and admin dashboard.
- **[obsicat.com](https://obsicat.com)** — My research portfolio. Pure HTML/CSS, zero dependencies, deployed on Vercel.

## Tech Stack

**Research & ML:** Python, PyTorch, JAX, Waymo Open Dataset, CARLA, CUDA, Transformers, LSTM, GNN, YOLOv8, PointPillars

**Engineering:** TypeScript, Next.js, React, Three.js, Node.js, Stripe, Supabase, PostgreSQL, Docker, Vercel

**3D & Creative:** Blender, ZBrush, Godot, ComfyUI, Stable Diffusion, LoRA training

**Tools:** Linux, Git, Neovim, Claude Code

## Links

[![Website](https://img.shields.io/badge/obsicat.com-Portfolio-1a2940?style=flat-square)](https://obsicat.com)
[![Email](https://img.shields.io/badge/Email-zhouxingnan2016@gmail.com-4ECDC4?style=flat-square)](mailto:zhouxingnan2016@gmail.com)
[![NudiLab](https://img.shields.io/badge/NudiLab-nudilab.art-d98c70?style=flat-square)](https://nudilab.art)
