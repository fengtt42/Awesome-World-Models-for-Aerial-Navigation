# Awesome World Models for Aerial Navigation
---

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![arXiv](https://img.shields.io/badge/arXiv-Papers-b31b1b.svg)](https://arxiv.org/abs/2509.20021)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://arxiv.org/abs/2502.05907)

<p align="center">
  <img src="Overview.png" alt="Awesome World Models for Aerial Navigation" width="100%">
</p>

A repository for aerial world models and UAV embodied navigation, covering methods, benchmarks, datasets, simulators, and workshops.

**Quick Links:** [Tasks](#tasks) · [Surveys](#Surveys) · [Aerial World Models](#AWM) · [Aerial Embodied Navigation](#AEN) · [Datasets & Benchmarks](#datasets) · [Simulators](#sim)

---

<a id="tasks"></a>
## Aerial Navigation Task

This repository prioritizes **aerial world models** and **UAV embodied navigation**. Pure mapping, detection, segmentation, VQA abd remote sensing works are included only when they directly support embodied navigation, benchmark construction, simulator development, or world-model training.

| Task | Name | Precise Definition |
| --- | --- | --- |
| `PointNav` | Point-goal Navigation | The UAV is given a geometric goal, such as a 2D/3D coordinate, waypoint, or relative displacement, and must reach the target location from an unseen start pose using onboard observations and executable motion actions. |
| `ImageNav` | Image-goal Navigation | The UAV is given a goal image depicting a target place, view, landmark, or object instance, and must navigate to the physical location or viewpoint that matches the image under viewpoint, scale, and appearance changes. |
| `ObjectNav` | Object-goal Navigation | The UAV is given a semantic object goal, object category, object description, or target instance, and must search for, localize, and stop near the target object in an unseen aerial environment. |
| `VLN` | Vision-and-Language Navigation | The UAV receives natural-language navigation instructions or goal descriptions and must ground them in visual observations, reason over aerial spatial relations, and execute sequential actions to reach the instructed destination. |
<p align="center">
  <img src="Tasks.png" alt="Awesome World Models for Aerial Navigation" width="100%">
</p>

---

## Surveys

| Date | Venue | Paper | Links |
| --- | --- | --- | --- |
| 2026-04 | arXiv | Vision-Language Navigation for Aerial Robots: Towards the Era of Large Language Models | [Paper](https://arxiv.org/abs/2604.07705) |
| 2025-02 | arXiv | The Role of World Models in Shaping Autonomous Driving: A Comprehensive Survey | [Paper](https://arxiv.org/abs/2502.10498) [Repo](https://github.com/LMD0311/Awesome-World-Model) |
| 2024-03 | arXiv | World Models for Autonomous Driving: An Initial Survey | [Paper](https://arxiv.org/abs/2403.02622) |
| 2023-12 | arXiv | Foundation Models in Robotics: Applications, Challenges, and the Future | [Paper](https://arxiv.org/abs/2312.07843) [Repo](https://github.com/robotics-survey/Awesome-Robotics-Foundation-Models) |

<a id="AWM"></a>
## Aerial World Models

| Date | Venue | Paper | Links |
| --- | --- | --- | --- |
| 2026-06 | arXiv | WorldFly: A World-Model-Based Vision-Language-Action Model for UAV Navigation | [Paper](https://arxiv.org/abs/2606.06147) |
| 2026-05 | arXiv | Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls | [Paper](https://arxiv.org/abs/2605.19728) |
| 2026-05 | arXiv | WorldVLN: Autoregressive World Action Model for Aerial Vision-Language Navigation | [Paper](https://arxiv.org/abs/2605.15964) [Project](https://embodiedcity.github.io/WorldVLN/) |
| 2025-12 | arXiv | Aerial World Model for Long-horizon Visual Generation and Navigation in 3D Space | [Paper](https://arxiv.org/abs/2512.21887) |
| 2025-09 | arXiv | FlightDiffusion: Revolutionising Autonomous Drone Training with Diffusion Models Generating FPV Video | [Paper](https://arxiv.org/abs/2509.14082) |
| 2025-07 | ACM MM | AirScape: An Aerial Generative World Model with Motion Controllability | [Paper](https://arxiv.org/abs/2507.08885) [Code](https://github.com/EmbodiedCity/AirScape.code) [Project](https://embodiedcity.github.io/AirScape/) [Dataset](https://huggingface.co/datasets/EmbodiedCity/AirScape-Dataset) |

<a id="AEN"></a>
## Aerial Embodied Navigation

| Date | Venue | Paper | Links |
| --- | --- | --- | --- |
| 2026-05 | arXiv | ESARBench: A Benchmark for Agentic UAV Embodied Search and Rescue | [Paper](https://arxiv.org/abs/2605.01371) [Project](https://4amgodvzx.github.io/ESAR.github.io/) |
| 2026-03 | arXiv | UAVBench and UAVIT-1M: Benchmarking and Enhancing MLLMs for Low-Altitude UAV Vision-Language Understanding | [Paper](https://arxiv.org/abs/2603.14336) [Project](https://UAVBench.github.io/) |
| 2026-02 | arXiv | APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation | [Paper](https://arxiv.org/abs/2602.00551) [Code](https://github.com/4amGodvzx/apex) |
| 2026-01 | arXiv | AirNav: A Large-Scale Real-World UAV Vision-and-Language Navigation Dataset with Natural and Diverse Instructions | [Paper](https://arxiv.org/abs/2601.03707) |
| 2025-12 | arXiv | MM-UAVBench: How Well Do Multimodal Large Language Models See, Think, and Plan in Low-Altitude UAV Scenarios? | [Paper](https://arxiv.org/abs/2512.23219) |
| 2025-11 | arXiv | OpenVLN: Open-world aerial Vision-Language Navigation | [Paper](https://arxiv.org/abs/2511.06182) |
| 2025-11 | arXiv | UAVBench: An Open Benchmark Dataset for Autonomous and Agentic AI UAV Systems via LLM-Generated Flight Scenarios | [Paper](https://arxiv.org/abs/2511.11252) [Code](https://github.com/maferrag/UAVBench) |
| 2025-11 | arXiv | AirCopBench: A Benchmark for Multi-drone Collaborative Embodied Perception and Reasoning | [Paper](https://arxiv.org/abs/2511.11025) |
| 2025-08 | arXiv | UAV-ON: A Benchmark for Open-World Object Goal Navigation with Aerial Agents | [Paper](https://arxiv.org/abs/2508.00288) |
| 2025-07 | arXiv | RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning | [Paper](https://arxiv.org/abs/2507.20776) |
| 2025-05 | arXiv | LogisticsVLN: Vision-Language Navigation For Low-Altitude Terminal Delivery Based on Agentic UAVs | [Paper](https://arxiv.org/abs/2505.03460) |
| 2025-04 | arXiv | UAV-VLN: End-to-End Vision Language guided Navigation for UAVs | [Paper](https://arxiv.org/abs/2504.21432) |
| 2024-11 | arXiv | NavAgent: Multi-scale Urban Street View Fusion For UAV Embodied Vision-and-Language Navigation | [Paper](https://arxiv.org/abs/2411.08579) |
| 2024-08 | arXiv | AeroVerse: UAV-Agent Benchmark Suite for Simulating, Pre-training, Finetuning, and Evaluating Aerospace Embodied World Models | [Paper](https://arxiv.org/abs/2408.15511) |
| 2023-11 | arXiv | GeoChat: Grounded Large Vision-Language Model for Remote Sensing | [Paper](https://arxiv.org/abs/2311.15826) [Code](https://github.com/mbzuai-oryx/geochat) |
| 2023-08 | ICCV | AerialVLN: Vision-and-Language Navigation for UAVs | [Paper](https://arxiv.org/abs/2308.06735) [Code](https://github.com/AirVLN/AirVLN) |

---

## Datasets & Benchmarks

| Date | Venue | Dataset / Benchmark | Task | Note | Links |
| --- | --- | --- | --- | --- | --- |
| 2026-05 | arXiv | ESARBench | ObjectNav | Search-and-rescue target finding in aerial scenes | [Paper](https://arxiv.org/abs/2605.01371) [Project](https://4amgodvzx.github.io/ESAR.github.io/) |
| 2026-02 | arXiv | APEX | ObjectNav | APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation | [Paper](https://arxiv.org/abs/2602.00551) [Code](https://github.com/4amGodvzx/apex) |
| 2026-01 | arXiv | AirNav | VLN | Real-world UAV navigation with natural language instructions | [Paper](https://arxiv.org/abs/2601.03707) |
| 2025-11 | arXiv | TravelUAV / OpenVLN | VLN | Open-world aerial vision-language navigation | [Paper](https://arxiv.org/abs/2511.06182) |
| 2025-08 | arXiv | UAV-ON | ObjectNav | Open-world object goal navigation for aerial agents | [Paper](https://arxiv.org/abs/2508.00288) |
| 2025-05 | arXiv | LogisticsVLN | VLN | Language-guided UAV delivery navigation | [Paper](https://arxiv.org/abs/2505.03460) |
| 2025-04 | arXiv | UAV-VLN | VLN | End-to-end vision-language guided UAV navigation | [Paper](https://arxiv.org/abs/2504.21432) |
| 2024-08 | arXiv | AeroVerse Navigation Tasks | PointNav | Navigation task suite for UAV agents | [Paper](https://arxiv.org/abs/2408.15511) |
| 2024-08 | arXiv | AeroVerse Visual Goal Tasks | ImageNav | Visual-goal style navigation tasks for UAV agents | [Paper](https://arxiv.org/abs/2408.15511) |
| 2023-08 | ICCV | AerialVLN | VLN | City-scale UAV VLN simulator and benchmark | [Code](https://github.com/AirVLN/AirVLN) [Paper](https://arxiv.org/abs/2308.06735) |

## Related Dataset

| Date | Venue | Dataset / Resource | Data Type | Note | Links |
| --- | --- | --- | --- | --- | --- |
| 2026-05 | arXiv | AeroBench | Generation | Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls | [Paper](https://arxiv.org/abs/2605.19728) |
| 2026-03 | arXiv | UAVBench + UAVIT-1M | Understanding | UAVBench and UAVIT-1M: Benchmarking and Enhancing MLLMs for Low-Altitude UAV Vision-Language Understanding | [Paper](https://arxiv.org/abs/2603.14336) [Project](https://UAVBench.github.io/) |
| 2025-12 | arXiv | ANWM / Aerial World Model data | Generation | Aerial World Model for Long-horizon Visual Generation and Navigation in 3D Space | [Paper](https://arxiv.org/abs/2512.21887) |
| 2025-12 | arXiv | MM-UAVBench | Understanding | MM-UAVBench: How Well Do Multimodal Large Language Models See, Think, and Plan in Low-Altitude UAV Scenarios? | [Paper](https://arxiv.org/abs/2512.23219) |
| 2025-07 | ACM MM | AirScape Dataset | Generation | AirScape: An Aerial Generative World Model with Motion Controllability | [Dataset](https://huggingface.co/datasets/EmbodiedCity/AirScape-Dataset) [Project](https://embodiedcity.github.io/AirScape/) |
| 2021-06 | arXiv | LoveDA | Segmentation | LoveDA: A Remote Sensing Land-Cover Dataset for Domain Adaptive Semantic Segmentation | [Code](https://github.com/Junjue-Wang/LoveDA) |
| 2020-01 | arXiv | VisDrone | Detection / Tracking | Vision Meets Drones: Past, Present and Future | [Dataset](https://github.com/VisDrone/VisDrone-Dataset) |
| 2019-05 | CVPRW | iSAID | Segmentation | iSAID: A Large-scale Dataset for Instance Segmentation in Aerial Images | [Website](https://captain-whu.github.io/iSAID/) |
| 2018-10 | arXiv | UAVid | Segmentation | UAVid: A Semantic Segmentation Dataset for UAV Imagery | [Website](https://uavid.nl/) [Paper](https://arxiv.org/abs/1810.10438) |
| 2018-04 | arXiv | UAVDT | Detection / Tracking | The Unmanned Aerial Vehicle Benchmark: Object Detection and Tracking | [Paper](https://arxiv.org/abs/1804.00518) |
| 2018-02 | arXiv | xView | Detection | xView: Objects in Context in Overhead Imagery | [Paper](https://arxiv.org/abs/1802.07856) |
| 2017-11 | CVPR / arXiv | DOTA | Detection | DOTA: A Large-scale Dataset for Object Detection in Aerial Images | [Website](https://captain-whu.github.io/DOTA/) [Paper](https://arxiv.org/abs/1711.10398) |

---

<a id="Sim"></a>
## Simulators

| Tool | Type | Good For | Links |
| --- | --- | --- | --- |
| AirSim | Unreal / Unity simulator | Photorealistic UAV simulation, data collection, APIs | [Code](https://github.com/microsoft/AirSim) [Docs](https://microsoft.github.io/AirSim/) [Paper](https://arxiv.org/abs/1705.05065) |
| Flightmare | Unity + physics quadrotor simulator | RL, planning, visual-inertial odometry | [Code](https://github.com/uzh-rpg/flightmare) [Website](https://uzh-rpg.github.io/flightmare/) [Paper](https://arxiv.org/abs/2009.00563) |
| gym-pybullet-drones | PyBullet / Gymnasium | Single/multi-agent quadcopter control and RL | [Code](https://github.com/learnsyslab/gym-pybullet-drones) [Paper](https://arxiv.org/abs/2103.02142) |
| PyFlyt | PyBullet / Gymnasium / PettingZoo | UAV RL and multi-agent experiments | [Code](https://github.com/jjshoots/PyFlyt) [Docs](https://taijunjet.com/PyFlyt/documentation.html) |

---

<a id="WS"></a>
## Workshops

| Year | Event | Topic | Links |
| --- | --- | --- | --- |
| 2025 | CVPR Workshop & Challenge, OpenDriveLab | World models and embodied navigation | [Website](https://opendrivelab.com/challenge25/#1x-wm) |
| 2025 | World Model Bench @ CVPR | Benchmarking world models | [Website](https://worldmodelbench.github.io/) |

---

Awesome World Models for Aerial Navigation.
