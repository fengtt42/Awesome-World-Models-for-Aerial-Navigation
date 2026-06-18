# Awesome World Models for Aerial Navigation

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![arXiv](https://img.shields.io/badge/arXiv-Papers-b31b1b.svg)](https://arxiv.org/abs/2509.20021)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://arxiv.org/abs/2502.05907)

<p align="center">
  <img src="Overview.png" alt="Awesome World Models for Aerial Navigation" width="100%">
</p>

This repo is used for recording, tracking, and benchmarking several recent World Models for Aerial Navigation methods, as a supplement to our [ACM MM 2024 Best Paper Nomination](https://arxiv.org/abs/2408.00606).

If you find some ignored papers, **feel free to _[create pull requests](#)_, or _[open issues](#)_**. Contributions in any form to make this list more comprehensive are welcome. 🫵 🫵 🫵

If you find this repository useful, please consider **giving us a star 🌟 and a [cite](#)**.

**Quick Links:** [Tasks](#tasks) · [Surveys](#Surveys) · [Aerial World Models](#AWM) · [Aerial Embodied Navigation](#AEN) · [Datasets & Benchmarks](#datasets) · [Simulators](#sim)


<a id="tasks"></a>
## Aerial Navigation Task

This repository prioritizes **aerial world models** and **UAV embodied navigation**. Pure mapping, detection, segmentation, VQA abd remote sensing works are included only when they directly support embodied navigation, benchmark construction, simulator development, or world-model training.

| Task | Name | Precise Definition |
| --- | --- | --- |
| `PointNav` | Point-goal Navigation | The UAV is given a geometric goal, such as a 2D/3D coordinate, waypoint, or relative displacement, and must reach the target location from an unseen start pose using onboard observations and executable motion actions. |
| `ImageNav` | Image-goal Navigation | The UAV is given a goal image depicting a target place, view, landmark, or object instance, and must navigate to the physical location or viewpoint that matches the image under viewpoint, scale, and appearance changes. |
| `ObjectNav` | Object-goal Navigation | The UAV is given a semantic object goal, object category, object description, or target instance, and must search for, localize, and stop near the target object in an unseen aerial environment. |
| `VLN` | Vision-and-Language Navigation | The UAV receives natural-language navigation instructions or goal descriptions and must ground them in visual observations, reason over aerial spatial relations, and execute sequential actions to reach the instructed destination. |
<!-- <p align="center">
  <img src="Tasks.png" alt="Awesome World Models for Aerial Navigation" width="100%">
</p> -->


## Surveys

| Date | Venue | Paper | Links |
| --- | --- | --- | --- |
| 26.04 | arXiv | Vision-Language Navigation for Aerial Robots: Towards the Era of Large Language Models | [Paper](https://arxiv.org/abs/2604.07705) |
| 25.02 | arXiv | The Role of World Models in Shaping Autonomous Driving: A Comprehensive Survey | [Paper](https://arxiv.org/abs/2502.10498) [Repo](https://github.com/LMD0311/Awesome-World-Model) |
| 24.03 | arXiv | World Models for Autonomous Driving: An Initial Survey | [Paper](https://arxiv.org/abs/2403.02622) |
| 23.12 | arXiv | Foundation Models in Robotics: Applications, Challenges, and the Future | [Paper](https://arxiv.org/abs/2312.07843) [Repo](https://github.com/robotics-survey/Awesome-Robotics-Foundation-Models) |

<a id="AWM"></a>
## Aerial World Models


| Date | Venue | Paper | Links |
| --- | --- | --- | --- |
| 26.06 | arXiv | MAD: Mapping-Aware World Models for Agile Quadrotor Flight | [Paper](https://arxiv.org/abs/2606.04534) |
| 26.06 | arXiv | AirDreamer: Generalist Drone Navigation with World Models | [Paper](https://arxiv.org/abs/2606.03252) |
| 26.06 | arXiv | ImagineUAV: Aerial Vision-Language Navigation via World-Action Modeling and Kinodynamic Planning | [Paper](https://arxiv.org/abs/2606.01205) |
| 26.06 | arXiv | WorldFly: A World-Model-Based Vision-Language-Action Model for UAV Navigation | [Paper](https://arxiv.org/abs/2606.06147) |
| 26.05 | arXiv | DeTrack: A Benchmark and Altitude-Aware Dual World Model for Drone-embodied Tracking | [Paper](https://arxiv.org/abs/2605.17451) |
| 26.05 | arXiv | Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls | [Paper](https://arxiv.org/abs/2605.19728) |
| 26.05 | arXiv | FlyMirage: A Fully Automated Generation Pipeline for Diverse and Scalable UAV Flight Data via Generative World Model | [Paper](https://arxiv.org/abs/2605.19600) |
| 26.05 | arXiv | WorldVLN: Autoregressive World Action Model for Aerial Vision-Language Navigation | [Paper](https://arxiv.org/abs/2605.15964) [Project](https://embodiedcity.github.io/WorldVLN/) |
| 25.12 | arXiv | Aerial World Model for Long-horizon Visual Generation and Navigation in 3D Space | [Paper](https://arxiv.org/abs/2512.21887) |
| 25.09 | arXiv | FlightDiffusion: Revolutionising Autonomous Drone Training with Diffusion Models Generating FPV Video | [Paper](https://arxiv.org/abs/2509.14082) |
| 25.07 | ACM MM | AirScape: An Aerial Generative World Model with Motion Controllability | [Paper](https://arxiv.org/abs/2507.08885) [Code](https://github.com/EmbodiedCity/AirScape.code) [Project](https://embodiedcity.github.io/AirScape/) [Dataset](https://huggingface.co/datasets/EmbodiedCity/AirScape-Dataset) |

<a id="AEN"></a>
## Aerial Embodied Navigation

| Date | Venue | Paper | Links |
| --- | --- | --- | --- |
| 26.05 | arXiv | ESARBench: A Benchmark for Agentic UAV Embodied Search and Rescue | [Paper](https://arxiv.org/abs/2605.01371) [Project](https://4amgodvzx.github.io/ESAR.github.io/) |
| 26.03 | arXiv | UAVBench and UAVIT-1M: Benchmarking and Enhancing MLLMs for Low-Altitude UAV Vision-Language Understanding | [Paper](https://arxiv.org/abs/2603.14336) [Project](https://UAVBench.github.io/) |
| 26.02 | arXiv | APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation | [Paper](https://arxiv.org/abs/2602.00551) [Code](https://github.com/4amGodvzx/apex) |
| 26.01 | arXiv | AirNav: A Large-Scale Real-World UAV Vision-and-Language Navigation Dataset with Natural and Diverse Instructions | [Paper](https://arxiv.org/abs/2601.03707) |
| 25.12 | arXiv | MM-UAVBench: How Well Do Multimodal Large Language Models See, Think, and Plan in Low-Altitude UAV Scenarios? | [Paper](https://arxiv.org/abs/2512.23219) |
| 25.11 | arXiv | OpenVLN: Open-world aerial Vision-Language Navigation | [Paper](https://arxiv.org/abs/2511.06182) |
| 25.11 | arXiv | UAVBench: An Open Benchmark Dataset for Autonomous and Agentic AI UAV Systems via LLM-Generated Flight Scenarios | [Paper](https://arxiv.org/abs/2511.11252) [Code](https://github.com/maferrag/UAVBench) |
| 25.11 | arXiv | AirCopBench: A Benchmark for Multi-drone Collaborative Embodied Perception and Reasoning | [Paper](https://arxiv.org/abs/2511.11025) |
| 25.08 | arXiv | UAV-ON: A Benchmark for Open-World Object Goal Navigation with Aerial Agents | [Paper](https://arxiv.org/abs/2508.00288) |
| 25.07 | arXiv | RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning | [Paper](https://arxiv.org/abs/2507.20776) |
| 25.06 | arXiv | Grounded Vision-Language Navigation for UAVs with Open-Vocabulary Goal Understanding | [Paper](https://arxiv.org/abs/2506.10756) |
| 25.05 | arXiv | LogisticsVLN: Vision-Language Navigation For Low-Altitude Terminal Delivery Based on Agentic UAVs | [Paper](https://arxiv.org/abs/2505.03460) |
| 25.04 | arXiv | UAV-VLN: End-to-End Vision Language guided Navigation for UAVs | [Paper](https://arxiv.org/abs/2504.21432) |
| 24.11 | arXiv | NavAgent: Multi-scale Urban Street View Fusion For UAV Embodied Vision-and-Language Navigation | [Paper](https://arxiv.org/abs/2411.08579) |
| 24.08 | arXiv | AeroVerse: UAV-Agent Benchmark Suite for Simulating, Pre-training, Finetuning, and Evaluating Aerospace Embodied World Models | [Paper](https://arxiv.org/abs/2408.15511) |
| 23.11 | arXiv | GeoChat: Grounded Large Vision-Language Model for Remote Sensing | [Paper](https://arxiv.org/abs/2311.15826) [Code](https://github.com/mbzuai-oryx/geochat) |
| 23.08 | ICCV | AerialVLN: Vision-and-Language Navigation for UAVs | [Paper](https://arxiv.org/abs/2308.06735) [Code](https://github.com/AirVLN/AirVLN) |



## Navigation Datasets & Benchmarks

| Date | Venue | Data & Bench | Task | Note | Links |
| --- | --- | --- | --- | --- | --- |
| 26.05 | arXiv | [ESARBench](https://arxiv.org/abs/2605.01371) | ObjectNav | ESARBench: A Benchmark for Agentic UAV Embodied Search and Rescue | [Project](https://4amgodvzx.github.io/ESAR.github.io/) |
| 26.02 | arXiv | [APEX](https://arxiv.org/abs/2602.00551) | ObjectNav | APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation | [Code](https://github.com/4amGodvzx/apex) |
| 26.02 | AAAI | [U2UData+](https://ojs.aaai.org/index.php/AAAI/article/view/37158) | ObjectNav | U2UData+: A Scalable Swarm UAVs Autonomous Flight Dataset for Embodied Long-horizon Tasks | [Project](https://fengtt42.github.io/U2UData-2/) [Code](https://github.com/fengtt42/U2UData-2) [Dataset](https://fengtt42.github.io/U2UData-2/) |
| 26.01 | arXiv | [AirNav](https://arxiv.org/abs/2601.03707) | VLN | AirNav: A Large-Scale Real-World UAV Vision-and-Language Navigation Dataset with Natural and Diverse Instructions |  |
| 25.12 | arXiv | [OpenVLN](https://arxiv.org/abs/2511.06182) | VLN | OpenVLN: Open-world Aerial Vision-Language Navigation |  |
| 25.08 | ACM MM | [UAV-ON](https://arxiv.org/abs/2508.00288) | ObjectNav | UAV-ON: A Benchmark for Open-World Object Goal Navigation with Aerial Agents |  |
| 25.05 | arXiv | [LogisticsVLN](https://arxiv.org/abs/2505.03460) | VLN | LogisticsVLN: Vision-Language Navigation For Low-Altitude Terminal Delivery Based on Agentic UAVs |  |
| 25.05 | arXiv | [CityAVOS](https://arxiv.org/abs/2505.08765) | ObjectNav | CityAVOS: Towards Autonomous UAV Visual Object Search in City Space |  |
| 25.04 | arXiv | [UAV-VLN](https://arxiv.org/abs/2504.21432) | VLN | UAV-VLN: End-to-End Vision Language Guided Navigation for UAVs |  |
| 25.02 | arXiv | [OpenFly](https://arxiv.org/abs/2502.18041) | VLN | OpenFly: A Versatile Toolchain and Large-scale Benchmark for Aerial Vision-Language Navigation | [Project](https://shailab-ipec.github.io/openfly/) [Code](https://github.com/Eziotic/OpenFly) |
| 25 | ICCV | [CityNav](https://arxiv.org/abs/2406.14240) | VLN | CityNav: A Large-Scale Dataset for Real-World Aerial Navigation | [Project](https://water-cookie.github.io/city-nav-proj/) [Code](https://github.com/water-cookie/citynav-arxiv) |
| 24.10 | ICLR | [OpenUAV](https://arxiv.org/abs/2410.07087) | ObjectNav / VLN | Towards Realistic UAV Vision-Language Navigation: Platform, Benchmark, and Methodology | [Project](https://prince687028.github.io/OpenUAV/) [Code](https://github.com/buaa-colalab/TravelUAV) |
| 24.08 | ACM MM | [U2UData](https://arxiv.org/abs/2408.00606) | ObjectNav | U2UData: A Large-scale Cooperative Perception Dataset for Swarm UAVs Autonomous Flight | [ACM](https://dl.acm.org/doi/10.1145/3664647.3681151) [Code](https://github.com/fengtt42/U2UData) [Dataset](https://github.com/fengtt42/U2UData) |
| 24.08 | arXiv | [AeroVerse](https://arxiv.org/abs/2408.15511) | PN / IN / VLN | AeroVerse: UAV-Agent Benchmark Suite for Simulating, Pre-training, Finetuning, and Evaluating Aerospace Embodied World Models |  |
| 23.08 | ICCV | [AerialVLN](https://arxiv.org/abs/2308.06735) | VLN | AerialVLN: Vision-and-Language Navigation for UAVs | [Code](https://github.com/AirVLN/AirVLN) [Dataset](https://github.com/AirVLN/AirVLN) |
| 20.10 | ACM MM | [University-1652](https://dl.acm.org/doi/10.1145/3394171.3413896) | ImageNav | University-1652: A Multi-view Multi-source Benchmark for Drone-based Geo-localization | [Code](https://github.com/layumi/University1652-Baseline) [Dataset](https://github.com/layumi/University1652-Baseline) |


## Aerial Other Dataset

| Date | Venue | Dataset / Resource | Data Type | Note | Links |
| --- | --- | --- | --- | --- | --- |
| 26.05 | arXiv | [AeroBench](https://arxiv.org/abs/2605.19728) | Generation | Aero-World: Action-Conditioned Aerial Video Generation from Inertial Controls |  |
| 26.03 | arXiv | [UAVBench + UAVIT-1M](https://arxiv.org/abs/2603.14336) | Vision-Language Understanding | UAVBench and UAVIT-1M: Benchmarking and Enhancing MLLMs for Low-Altitude UAV Vision-Language Understanding | [Project](https://UAVBench.github.io/) |
| 25.12 | arXiv | [ANWM](https://arxiv.org/abs/2512.21887) | Generation / Navigation Support | Aerial World Model for Long-horizon Visual Generation and Navigation in 3D Space |  |
| 25.12 | arXiv | [MM-UAVBench](https://arxiv.org/abs/2512.23219) | Vision-Language Understanding / Planning | MM-UAVBench: How Well Do Multimodal Large Language Models See, Think, and Plan in Low-Altitude UAV Scenarios? |  |
| 25.07 | ACM MM | [AirScape](https://arxiv.org/abs/2507.08885) | Generation / World Model | AirScape: An Aerial Generative World Model with Motion Controllability | [Project](https://embodiedcity.github.io/AirScape/) [Code](https://github.com/EmbodiedCity/AirScape.code) [Dataset](https://huggingface.co/datasets/EmbodiedCity/AirScape-Dataset) |
| 25.07 | arXiv | [RingMo-Agent](https://arxiv.org/abs/2507.20776) | Remote Sensing Reasoning | RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning |  |
| 24.08 | NeurIPS Datasets and Benchmarks | [UAV3D](https://arxiv.org/abs/2410.11125) | 3D Perception | UAV3D: A Large-scale 3D Perception Benchmark for Unmanned Aerial Vehicles | [Project](https://huiyegit.github.io/UAV3D_Benchmark/) [Code](https://github.com/huiyegit/UAV3D) |
| 23.11 | arXiv | [GeoChat Dataset](https://arxiv.org/abs/2311.15826) | Remote Sensing VQA / Reasoning | GeoChat: Grounded Large Vision-Language Model for Remote Sensing | [Code](https://github.com/mbzuai-oryx/geochat) |
| 21.06 | arXiv | [LoveDA](https://arxiv.org/abs/2110.08733) | Segmentation | LoveDA: A Remote Sensing Land-Cover Dataset for Domain Adaptive Semantic Segmentation | [Code](https://github.com/Junjue-Wang/LoveDA) |
| 20.01 | arXiv | [VisDrone](https://github.com/VisDrone/VisDrone-Dataset) | Detection / Tracking | Vision Meets Drones: A Challenge | |
| 19.05 | CVPRW | [iSAID](https://captain-whu.github.io/iSAID/) | Instance Segmentation | iSAID: A Large-scale Dataset for Instance Segmentation in Aerial Images |  |
| 18.10 | arXiv | [UAVid](https://arxiv.org/abs/1810.10438) | Semantic Segmentation | UAVid: A Semantic Segmentation Dataset for UAV Imagery | [Website](https://uavid.nl/) |
| 18.04 | ECCV / arXiv | [UAVDT](https://arxiv.org/abs/1804.00518) | Detection / Tracking | The Unmanned Aerial Vehicle Benchmark: Object Detection and Tracking |  |
| 18.02 | arXiv | [xView](https://arxiv.org/abs/1802.07856) | Detection | xView: Objects in Context in Overhead Imagery |  |
| 17.11 | CVPR / arXiv | [DOTA](https://arxiv.org/abs/1711.10398) | Detection | DOTA: A Large-scale Dataset for Object Detection in Aerial Images | [Website](https://captain-whu.github.io/DOTA/) |


---

<a id="Sim"></a>
## Simulators

| Simulator | Type | Good For | Links |
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
