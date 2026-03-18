# Awesome Humanoid & Dexterous Manipulation
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-red.svg)](https://github.com/chetanraj/awesome-github-badges)

A curated list of awesome papers and resources on **humanoid manipulation**, **dexterous manipulation**, **bimanual dexterous manipulation**, and **humanlike manipulation**. This repo covers upper-body humanoid robot learning, multi-fingered hand manipulation, in-hand object reorientation, and related topics. Inspired by [awesome-humanoid-learning](https://github.com/jonyzhang2023/awesome-humanoid-learning).

**Keywords**: awesome humanoid manipulation, awesome dexterous manipulation, awesome bimanual manipulation, awesome dexterous hand, awesome humanoid robot, awesome robot hand manipulation, in-hand manipulation, dexterous grasping

_Scope_: This list covers the following topics:

1. Humanoid robot manipulation and loco-manipulation
2. Dexterous hand manipulation (single-hand, in-hand reorientation, dexterous grasping)
3. Bimanual dexterous multi-fingered manipulation
4. Dual-arm manipulation with other end effectors
5. Teleoperation and human-to-robot retargeting for dexterous tasks
6. Physically simulated humanoid animations and digital human-object interaction

**Contributions are welcome!** Please feel free to submit a pull request or open an issue.

---

## Contents
- [Awesome Humanoid \& Dexterous Manipulation](#awesome-humanoid--dexterous-manipulation)
  - [Contents](#contents)
  - [Robot Models](#robot-models)
    - [Humanoids](#humanoids)
    - [Dexterous Hands](#dexterous-hands)
    - [Dual-Arm Robots](#dual-arm-robots)
  - [Simulation Environments \& Benchmarks](#simulation-environments--benchmarks)
  - [Workshops](#workshops)
  - [Projects](#projects)
  - [Packages](#packages)
  - [Related Awesome Lists](#related-awesome-lists)
  - [Papers](#papers)
    - [Surveys](#surveys)
    - [Humanoid Robot Manipulation](#humanoid-robot-manipulation)
    - [Dexterous Hand Manipulation](#dexterous-hand-manipulation)
    - [Bimanual Dexterous Multi-Fingered Manipulation](#bimanual-dexterous-multi-fingered-manipulation)
    - [Teleoperation \& Human-to-Robot Retargeting](#teleoperation--human-to-robot-retargeting)
    - [Dual-Arm Manipulation with Other End Effectors](#dual-arm-manipulation-with-other-end-effectors)
    - [Physically Simulated Humanoid Animations and Digital Human-Object Interaction](#physically-simulated-humanoid-animations-and-digital-human-object-interaction)


<a name="Models" />

## Robot Models

<a name="Humanoids" />

### Humanoids

| Name | Maker | Formats | License | Meshes | Inertias | Collisions |
|------|-------|---------|---------|--------|----------|------------|
| H1 | Unitree | [URDF & MJCF](https://github.com/unitreerobotics/unitree_ros/tree/master/robots/h1_description), [USD](https://github.com/unitreerobotics/unitree_model/tree/main/H1/usd) | BSD-3-Clause | ✔️ | ✔️ | ✔️ |
| H1-2 (preview) | Unitree | [URDF & MJCF](https://github.com/unitreerobotics/unitree_rl_gym/tree/main/resources/robots/h1_2), [Simplified URDF](https://github.com/unitreerobotics/unitree_rl_gym/tree/main/resources/robots/h1_2) | BSD-3-Clause | ✔️ | ✔️ | ✔️ |
| G1 | Unitree | [URDF & MJCF](https://github.com/unitreerobotics/unitree_ros/tree/master/robots/g1_description) | BSD-3-Clause | ✔️ | ✔️ | ✔️ |
| GR-1 | FFTAI (Fourier) | [URDF](https://github.com/FFTAI/Wiki-GRx-Models/tree/master/GRX/GR1), [MJCF](https://github.com/FFTAI/wiki-mjcf/) | GPL-3.0 | ✔️ | ✔️ | ✔️ |
| GR-2 | FFTAI (Fourier) | [URDF](https://github.com/FFTAI/Wiki-GRx-Models) | GPL-3.0 | ✔️ | ✔️ | ✔️ |
| AgiBot X1 | AgiBot | [URDF & MJCF](https://github.com/AgibotTech/agibot_x1_train) | Apache-2.0 | ✔️ | ✔️ | ✔️ |
| Atlas v4 | Boston Dynamics | [URDF](https://github.com/openai/roboschool/tree/1.0.49/roboschool/models_robot/atlas_description) | MIT | ✔️ | ✔️ | ✔️ |
| Digit | Agility Robotics | [URDF](https://github.com/adubredu/DigitRobot.jl/tree/main/urdf) | ✖️ | ✔️ | ✔️ | ✔️ |
| Magicbot Z1 | Magiclab | [URDF](https://github.com/MagiclabRobotics/magicbot-z1_description) | ✖️ | ✔️ | ✔️ | ✔️ |
| Deep Robotics | Deep Robotics | [URDF](https://github.com/DeepRoboticsLab/URDF_model) | ✖️ | ✔️ | ✔️ | ✔️ |

Also see: [MuJoCo Menagerie](https://github.com/google-deepmind/mujoco_menagerie) for high-quality MJCF models, [awesome-robot-descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions) for a comprehensive list.

<a name="DexterousHands" />

### Dexterous Hands

| Name | Maker | Formats | License | Meshes | Inertias | Collisions |
|------|-------|---------|---------|--------|----------|------------|
| Ability Hand | PSYONIC, Inc. | [MJCF](https://github.com/psyonicinc/ability-hand-api/tree/master/URDF/mujoco), [URDF](https://github.com/psyonicinc/ability-hand-api/tree/master/URDF) | ✖️ | ✔️ | ✔️ | ✖️ |
| Allegro Hand | Wonik Robotics | [URDF](https://github.com/RobotLocomotion/models/tree/master/allegro_hand_description/urdf), [MJCF](https://github.com/google-deepmind/mujoco_menagerie/tree/main/wonik_allegro) | BSD | ✔️ | ✔️ | ✔️ |
| Shadow Hand | Shadow Robot | [URDF](https://github.com/shadow-robot/sr_common/tree/noetic-devel/sr_description/mujoco_models/urdfs), [MJCF](https://github.com/google-deepmind/mujoco_menagerie/tree/main/shadow_hand) | BSD | ✔️ | ✔️ | ✔️ |
| LEAP Hand | Carnegie Mellon | [URDF](https://github.com/leap-hand/LEAP_Hand_Sim/tree/main/assets) | MIT | ✔️ | ✔️ | ✔️ |
| Inspire Hand | Inspire-Robots | [URDF](https://github.com/dexsuite/dex-urdf) | ✖️ | ✔️ | ✔️ | ✔️ |
| ORCA Hand | ORCA Robotics | [URDF & MJCF](https://github.com/orcahand/orcahand_description) | ✖️ | ✔️ | ✔️ | ✔️ |
| Wuji Hand | Wuji Technology | [URDF & MJCF](https://github.com/wuji-technology/wuji-hand-description) | ✖️ | ✔️ | ✔️ | ✔️ |
| SVH Hand | SCHUNK | [URDF](https://github.com/dexsuite/dex-urdf) | ✖️ | ✔️ | ✔️ | ✔️ |

Also see: [dex-urdf](https://github.com/dexsuite/dex-urdf) for a collection of dexterous hand URDFs.

<a name="DualArmRobots" />

### Dual-Arm Robots

| Name | Maker | Formats | License | Visuals | Inertias | Collisions |
|------|-------|---------|---------|---------|----------|------------|
| YuMi | ABB | [URDF](https://github.com/OrebroUniversity/yumi/tree/master/yumi_description) | BSD-2-Clause | ✔️ | ✔️ | ✔️ |
| Dual iiwa 14 | KUKA | [URDF](https://github.com/RobotLocomotion/models/blob/master/iiwa_description/urdf/dual_iiwa14_polytope_collision.urdf), [Xacro](https://github.com/RobotLocomotion/models/blob/master/iiwa_description/urdf/dual_iiwa14_polytope_collision.urdf.xacro) | BSD-3-Clause | ✔️ | ✔️ | ✔️ |
| ALOHA 2 | Google DeepMind | [URDF](https://github.com/google-deepmind/mujoco_menagerie/tree/main/google_robot) | Apache-2.0 | ✔️ | ✔️ | ✔️ |


<a name="SimulationEnvironments" />

## Simulation Environments & Benchmarks

| Name | Description | Link |
|------|-------------|------|
| ManiSkill | GPU-parallelized robotics simulator with dexterous manipulation tasks | [[github](https://github.com/haosulab/ManiSkill)] [[doc](https://www.maniskill.ai/)] |
| Isaac Lab | NVIDIA Isaac Sim-based robot learning framework with dexterous manipulation support | [[github](https://github.com/isaac-sim/IsaacLab)] |
| DexGraspNet | Large-scale robotic dexterous grasp dataset for general objects | [[github](https://github.com/PKU-EPIC/DexGraspNet)] [[paper](https://arxiv.org/abs/2210.02697)] |
| HumanoidBench | Simulated humanoid benchmark for whole-body locomotion and manipulation | [[github](https://github.com/carlosferrazza/humanoid-bench)] [[paper](https://arxiv.org/abs/2403.10506)] |
| BiGym | Demo-driven mobile bi-manual manipulation benchmark | [[github](https://github.com/chernyadev/bigym)] [[paper](https://arxiv.org/abs/2407.07788)] |
| GRUtopia | General robots in a city at scale | [[github](https://github.com/OpenRobotLab/GRUtopia)] [[paper](https://arxiv.org/abs/2407.10943)] |
| Humanoid-Gym | RL for humanoid robot with zero-shot sim2real transfer | [[github](https://github.com/roboterax/humanoid-gym)] [[paper](https://arxiv.org/abs/2404.05695)] |
| DexterousHands | Bi-level multi-agent RL for dexterous manipulation | [[github](https://github.com/PKU-MARL/DexterousHands)] |


<a name="Workshops" />

## Workshops

RSS 2025 [[3rd Workshop on Dexterous Manipulation: Learning and Control with Diverse Data](https://dex-manipulation.github.io/rss2025/)]

Humanoids 2025 [[Dexterous Humanoid Manipulation Workshop](https://dexterous-humanoid-manipulation.github.io/)]

CORL 2024 [[Workshop on Whole-body Control and Bimanual Manipulation: Applications in Humanoids and Beyond](https://wcbm-workshop.github.io/)]

RSS 2024 [[2nd Workshop on Dexterous Manipulation: Design, Perception and Control](https://dex-manipulation.github.io/rss2024/)]

<a name="Projects" />

## Projects

AgiBot-World [[AgiBot World: A Large-scale Manipulation Platform](https://agibot-world.com/)] [[github](https://github.com/OpenDriveLab/AgiBot-World)]

Lerobot [[LeRobot: State-of-the-art AI for real-world robotics](https://github.com/huggingface/lerobot)]

LEAP Hand [[A Low-Cost Dexterous Hand for Robot Learning](https://leaphand.com/)] [[github](https://github.com/leap-hand)]

DOGlove [[Low-Cost Haptic Force Feedback Glove](https://arxiv.org/abs/2502.07730)]

ACE Teleop [[Cross-Platform Visual-Exoskeletons for Low-Cost Dexterous Teleoperation](https://ace-teleop.github.io/)] [[github](https://github.com/ACETeleop/ACETeleop)]

<a name="Packages" />

## Packages

### Rofunc

Rofunc: The Full Process Python Package for Robot Learning from Demonstration and Robot Manipulation [[pkg](https://github.com/Skylark0924/Rofunc)] [[doc](https://rofunc.readthedocs.io/en/latest/)]

### dex-urdf

dex-urdf: A collection of high-quality URDF models for dexterous hands and objects [[pkg](https://github.com/dexsuite/dex-urdf)]

### robot_descriptions

robot_descriptions: Python package to load robot description files (URDF, MJCF) [[pkg](https://github.com/robot-descriptions/robot_descriptions.py)]


<a name="RelatedAwesomeLists" />

## Related Awesome Lists

- [Awesome-Dexterous-Manipulation](https://github.com/kingchou007/Awesome-Dexterous-Manipulation) - Resources on dexterous manipulation
- [Awesome-Loco-Manipulation](https://github.com/aCodeDog/awesome-loco-manipulation) - Locomotion and manipulation
- [Awesome-Robotics-Manipulation](https://github.com/BaiShuanghao/Awesome-Robotics-Manipulation) - Comprehensive robot manipulation papers
- [Awesome-What-Bimanual-Can-Do](https://github.com/xzxzxzxz/Awesome-What-Bimanual-Can-Do) - Bimanual manipulation
- [awesome-humanoid-learning](https://github.com/jonyzhang2023/awesome-humanoid-learning) - Humanoid robot learning
- [awesome-humanoid-robot-learning](https://github.com/YanjieZe/awesome-humanoid-robot-learning) - Humanoid robot learning papers
- [Awesome-Touch](https://github.com/linchangyi1/Awesome-Touch) - Tactile sensing and manipulation
- [awesome-robot-descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions) - URDF/MJCF robot models


<a name="Papers" />

## Papers

YYYY.MM is the date when paper appears on arxiv.org (if available).


<a name="Surveys" />

### Surveys

- [2025.04] Dexterous Manipulation through Imitation Learning: A Survey [[paper](https://arxiv.org/abs/2504.03515)]

- [2025.01] Humanoid Locomotion and Manipulation: Current Progress and Challenges in Control, Planning, and Learning [[paper](https://arxiv.org/abs/2501.02116)]


<a name="HumanoidRobotManipulation" />

### Humanoid Robot Manipulation

- [2026.03] HumDex: Humanoid Dexterous Manipulation Made Easy [**teleop**] [[paper](https://arxiv.org/abs/2603.12260)]

- [2025.11] VIRAL: Visual Sim-to-Real at Scale for Humanoid Loco-Manipulation [**RL**] [**sim2real**] [[paper](https://arxiv.org/abs/2511.15200)]

- [2025.10] DemoHLM: From One Demonstration to Generalizable Humanoid Loco-Manipulation [**IL**] [[paper](https://arxiv.org/abs/2510.11258)]

- [2025.09] DreamControl: Human-Inspired Whole-Body Humanoid Control for Scene Interaction via Guided Diffusion [**diffusion**] [[paper](https://arxiv.org/abs/2509.14353)]

- [2025.05] FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation [**RL**] [[paper](https://arxiv.org/abs/2505.06776)]

- [2025.05] Humanoid Loco-manipulation Planning based on Graph Search and Reachability Maps [**planning**] [[paper](https://arxiv.org/abs/2505.23505)]

- [2025.05] MaskedManipulator: Versatile Whole-Body Manipulation [**RL**] [[paper](https://arxiv.org/abs/2505.19086)]

- [2025.03] Humanoids in Hospitals: A Technical Study of Humanoid Surrogates for Dexterous Medical Interventions [[paper](https://arxiv.org/abs/2503.12725)] [[project](https://surgie-humanoid.github.io/)]

- [2025.03] Humanoid Policy ~ Human Policy [[paper](https://arxiv.org/abs/2503.13441)] [[project](https://human-as-robot.github.io/)]

- [2025.03] FLAM: Foundation Model-Based Body Stabilization for Humanoid Locomotion and Manipulation [[paper](https://arxiv.org/abs/2503.22249)] [[project](https://xianqi-zhang.github.io/FLAM/)]

- [2025.02] Sim-to-Real Reinforcement Learning for Vision-Based Dexterous Manipulation on Humanoids [**RL**] [**sim2real**] [[paper](https://arxiv.org/abs/2502.20396)]

- [2025.02] InterMimic: Towards Universal Whole-Body Control for Physics-Based Human-Object Interactions [**RL**] [[paper](https://arxiv.org/abs/2502.20390)]

- [2025.02] Dexterous Safe Control for Humanoids in Cluttered Environments via Projected Safe Set Algorithm [**Control**] [[project](https://toruowo.github.io/recipe/)] [[paper](https://arxiv.org/abs/2502.02858)]

- [2024.12] Mimicking-Bench: A Benchmark for Generalizable Humanoid-Scene Interaction Learning via Human Mimicking [**Benchmark**]  [[project](https://mimicking-bench.github.io/)] [[paper](https://arxiv.org/abs/2412.17730)]

- [2024.12] ARMOR: Egocentric Perception for Humanoid Robot Collision Avoidance and Motion Planning [**IL**] [**MP**] [[paper](https://arxiv.org/abs/2412.00396)]

- [2024.12] Mobile-TeleVision: Predictive Motion Priors for Humanoid Whole-Body Control [**RL**] [[project](https://mobile-tv.github.io/)] [[paper](https://arxiv.org/abs/2412.07773)] [[code](https://github.com/OpenTeleVision/TeleVision)]

- [2024.10] EgoMimic: Scaling Imitation Learning via Egocentric Video [**IL**] [[project](https://egomimic.github.io/)] [[paper](https://arxiv.org/abs/2410.24221)] [[code](https://github.com/SimarKareer/EgoMimic)]

- [2024.10] DexMimicGen: Automated Data Generation for Bimanual Dexterous Manipulation via Imitation Learning [**IL**] [[project](https://dexmimicgen.github.io/#)] [[paper](https://arxiv.org/abs/2410.24185)]

- [2024.10] OKAMI: Teaching Humanoid Robots Manipulation Skills through Single Video Imitation [**IL**] [[project](https://ut-austin-rpl.github.io/OKAMI/)] [[paper](http://arxiv.org/abs/2410.11792)]

- [2024.10] Generalizable Humanoid Manipulation with Improved 3D Diffusion Policies [**IL**] [**diffusion**] [[project](https://humanoid-manipulation.github.io/)] [[paper](https://arxiv.org/abs/2410.10803)] [[code](https://github.com/YanjieZe/Improved-3D-Diffusion-Policy)]

- [2024.08] RP1M: A Large-Scale Motion Dataset for Piano Playing with Bi-Manual Dexterous Robot Hands [**Dataset**] [[project](https://rp1m.github.io/)] [[paper](https://arxiv.org/abs/2408.11048)] [[code](https://github.com/google-research/robopianist)]

- [2024.07] Open-TeleVision Teleoperation with Immersive Active Visual Feedback [**teleop**] [[project](https://robot-tv.github.io/)] [[paper](https://arxiv.org/abs/2407.01512)] [[code](https://github.com/OpenTeleVision/TeleVision)]

- [2024.07] GRUtopia: Dream General Robots in a City at Scale [**benchmark**] [[doc](https://grutopia.github.io/)] [[paper](https://arxiv.org/abs/2407.10943)] [[code](https://github.com/OpenRobotLab/GRUtopia)]

- [2024.07] BiGym: A Demo-Driven Mobile Bi-Manual Manipulation Benchmark [**benchmark**] [[project](https://chernyadev.github.io/bigym)] [[paper](https://arxiv.org/abs/2407.07788)]

- [2024.06] HumanPlus: Humanoid Shadowing and Imitation from Humans [**IL**] [[project](https://humanoid-ai.github.io/)] [[paper](https://arxiv.org/abs/2406.10454)] [[code](https://github.com/MarkFzp/humanplus)]

- [2024.06] Learning Hybrid Behavior Planning for Autonomous Loco-manipulation [**VLM**] [[project](https://hy-motion.github.io/)] [[paper](https://arxiv.org/abs/2406.14655v1)]

- [2024.06] OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning [**benchmark**] [[project](https://omni.human2humanoid.com/)] [[paper](https://arxiv.org/abs/2406.08858)] [[code](https://github.com/LeCAR-Lab/human2humanoid)]

- [2024.04] Large Language Models for Orchestrating Bimanual Robots [**LLM**] [[paper](https://arxiv.org/abs/2404.02018)] [[project](https://labor-agent.github.io/)] [[code](https://github.com/Kchu/LABOR-Agent)]

- [2024.04] Humanoid-Gym: Reinforcement Learning for Humanoid Robot with Zero-Shot Sim2Real Transfer [**RL**] [**benchmark**] [[paper](https://arxiv.org/abs/2404.05695)] [[project](https://sites.google.com/view/humanoid-gym/)] [[code](https://github.com/roboterax/humanoid-gym)]

- [2024.03] HumanoidBench: Simulated Humanoid Benchmark for Whole-Body Locomotion and Manipulation [**benchmark**] [[project](https://humanoid-bench.github.io/)] [[paper](https://arxiv.org/abs/2403.10506)] [[code](https://github.com/carlosferrazza/humanoid-bench)]

- [2024.03] Bi-KVIL: Keypoints-based Visual Imitation Learning of Bimanual Manipulation Tasks [**IL**] [[project](https://sites.google.com/view/bi-kvil)] [[paper](https://arxiv.org/abs/2403.03270)] [[code](https://github.com/wyngjf/bi-kvil-pub)]


<a name="DexterousHandManipulation" />

### Dexterous Hand Manipulation

- [2026.02] DexRepNet++: Learning Dexterous Robotic Manipulation with Geometric and Spatial Hand-Object Representations [**RL**] [[paper](https://arxiv.org/abs/2602.21811)]

- [2026.02] UniMorphGrasp: Diffusion Model with Morphology-Awareness for Cross-Embodiment Dexterous Grasp Generation [**diffusion**] [[paper](https://arxiv.org/abs/2602.00915)]

- [2026.02] DexEvolve: Evolutionary Optimization for Robust and Diverse Dexterous Grasp Synthesis [**optimization**] [[paper](https://arxiv.org/abs/2602.15201)]

- [2026.02] SimToolReal: An Object-Centric Policy for Zero-Shot Dexterous Tool Manipulation [**RL**] [**sim2real**] [[paper](https://arxiv.org/abs/2602.16863)]

- [2026.01] Closing the Reality Gap: Zero-Shot Sim-to-Real Deployment for Dexterous Force-Based Grasping and Manipulation [**RL**] [**sim2real**] [[paper](https://arxiv.org/abs/2601.02778)]

- [2025.09] Dexplore: Scalable Neural Control for Dexterous Manipulation from Reference-Scoped Exploration [**RL**] [[paper](https://arxiv.org/abs/2509.09671)]

- [2025.09] In-Hand Manipulation of Articulated Tools with Dexterous Robot Hands with Sim-to-Real Transfer [**RL**] [**sim2real**] [[paper](https://arxiv.org/abs/2509.23075)]

- [2025.09] Learning Dexterous Manipulation with Quantized Hand State [**RL**] [[paper](https://arxiv.org/abs/2509.17450)]

- [2025.08] DexReMoE: In-hand Reorientation of General Object via Mixtures of Experts [**RL**] [[paper](https://arxiv.org/abs/2508.01695)]

- [2025.04] Multi-Goal Dexterous Hand Manipulation using Probabilistic Model-based Reinforcement Learning [**RL**] [[paper](https://arxiv.org/abs/2504.21585)]

- [2025.03] DexGrasp Anything: Towards Universal Robotic Dexterous Grasping with Physics Awareness [**diffusion**] [[paper](https://arxiv.org/abs/2503.08257)]

- [2025.03] Dexterous Hand Manipulation via Efficient Imitation-Bootstrapped Online Reinforcement Learning [**RL**] [**IL**] [[paper](https://arxiv.org/abs/2503.04014)]

- [2025.03] GenForce: Training Tactile Sensors to Learn Force Sensing from Each Other [**touch**] [[paper](https://arxiv.org/abs/2503.01058)]

- [2025.01] From Simple to Complex Skills: The Case of In-Hand Object Reorientation [**RL**] [**sim2real**] [[paper](https://arxiv.org/abs/2501.05439)]

- [2024.12] BODex: Scalable and Efficient Robotic Dexterous Grasp Synthesis Using Bilevel Optimization [**optimization**] [[paper](https://arxiv.org/abs/2412.16490)]

- [2024.12] Dexterous Manipulation Based on Prior Dexterous Grasp Pose Knowledge [**RL**] [[paper](https://arxiv.org/abs/2412.15587)]

- [2024.11] Object-Centric Dexterous Manipulation from Human Motion Data [**RL**] [[project](https://cypypccpy.github.io/obj-dex.github.io/)] [[paper](https://arxiv.org/abs/2411.04005)]


<a name="BimanualDexterousMulti-FingeredManipulation" />

### Bimanual Dexterous Multi-Fingered Manipulation

- [2026.01] DemoBot: Efficient Learning of Bimanual Manipulation with Dexterous Hands From Third-Person Human Videos [**RL**] [**IL**] [[paper](https://arxiv.org/abs/2601.01651)]

- [2025.10] DexMan: Learning Bimanual Dexterous Manipulation from Human and Generated Videos [**IL**] [[paper](https://arxiv.org/abs/2510.08475)]

- [2025.05] DexMachina: Functional Retargeting for Bimanual Dexterous Manipulation [**RL**] [[paper](https://arxiv.org/abs/2505.24853)]

- [2025.03] ManipTrans: Efficient Dexterous Bimanual Manipulation Transfer via Residual Learning [**IL**] [[paper](https://arxiv.org/abs/2503.21860)]

- [2024.12] GigaHands: A Massive Annotated Dataset of Bimanual Hand Activities [**Dataset**] [[project](https://ivl.cs.brown.edu/research/gigahands.html)] [[paper](https://arxiv.org/abs/2412.04244)]

- [2024.11] Bimanual Dexterity for Complex Tasks [**IL**] [[project](https://bidex-teleop.github.io/)] [[paper](https://openreview.net/pdf?id=55tYfHvanf)]

- [2024.10] Learning Diverse Bimanual Dexterous Manipulation Skills From Human [**IL**] [[project](https://sites.google.com/view/bidexhd)] [[paper](https://arxiv.org/abs/2410.02477)]

- [2024.07] Bunny-Vision Pro: Real-Time Bimanual Dexterous Teleoperation for Imitation Learning [**IL**] [[project](https://dingry.github.io/projects/bunny_visionpro)] [[paper](https://arxiv.org/abs/2407.03162)] [[code](https://github.com/Dingry/BunnyVisionPro)]

- [2024.04] Learning Visuotactile Skills with Two Multifingered Hands [**IL**] [**touch**] [[project](https://toruowo.github.io/hato/)] [[paper](http://arxiv.org/abs/2404.16823)] [[code](https://github.com/toruowo/hato)]

- [2024.03] DexCap: Scalable and Portable Mocap Data Collection System for Dexterous Manipulation [**IL**] [[project](https://dex-cap.github.io/)] [[paper](https://arxiv.org/abs/2403.07788)] [[code](https://github.com/j96w/DexCap)]


<a name="TeleoperationRetargeting" />

### Teleoperation & Human-to-Robot Retargeting

- [2025.12] GR-Dexter Technical Report [**teleop**] [[paper](https://arxiv.org/abs/2512.24210)]

- [2025.07] Dexterous Teleoperation of 20-DoF ByteDexter Hand via Human Motion Retargeting [**teleop**] [[paper](https://arxiv.org/abs/2507.03227)]

- [2025.07] TypeTele: Releasing Dexterity in Teleoperation by Dexterous Manipulation Types [**teleop**] [[paper](https://arxiv.org/abs/2507.01857)]

- [2025.07] Human-Exoskeleton Kinematic Calibration to Improve Hand Tracking for Dexterous Teleoperation [**teleop**] [[paper](https://arxiv.org/abs/2507.23592)]

- [2025.06] GEX: Democratizing Dexterity with Fully-Actuated Dexterous Hand and Exoskeleton Glove [**teleop**] [[paper](https://arxiv.org/abs/2506.04982)]

- [2025.05] TeleOpBench: A Simulator-Centric Benchmark for Dual-Arm Dexterous Teleoperation [**benchmark**] [**teleop**] [[paper](https://arxiv.org/abs/2505.12748)]

- [2025.05] DexUMI: Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation [**teleop**] [[paper](https://arxiv.org/abs/2505.21864)]

- [2025.03] Exo-ViHa: A Cross-Platform Exoskeleton System with Visual and Haptic Feedback [**teleop**] [[paper](https://arxiv.org/abs/2503.01543)]

- [2025.02] DOGlove: Dexterous Manipulation with a Low-Cost Open-Source Haptic Force Feedback Glove [**teleop**] [[paper](https://arxiv.org/abs/2502.07730)]

- [2024.08] ACE: A Cross-platform Visual-Exoskeletons for Low-Cost Dexterous Teleoperation [**teleop**] [[project](https://ace-teleop.github.io/)] [[paper](https://arxiv.org/abs/2408.11805)] [[code](https://github.com/ACETeleop/ACETeleop)]


<a name="DualArmManipulationwithOtherEndEffectors" />

### Dual-Arm Manipulation with Other End Effectors

- [2025.10] ManiDP: Manipulability-Aware Diffusion Policy for Posture-Dependent Bimanual Manipulation [**diffusion**] [[paper](https://arxiv.org/abs/2510.23016)]

- [2025.05] Towards a Generalizable Bimanual Foundation Policy via Flow-based Video Prediction [**IL**] [**foundation**] [[paper](https://arxiv.org/abs/2505.24156)]

- [2025.03] Learning Bimanual Manipulation via Action Chunking and Inter-Arm Coordination with Transformers [**IL**] [[paper](https://arxiv.org/abs/2503.13916)]

- [2025.01] YOTO: You Only Teach Once: Learn One-Shot Bimanual Robotic Manipulation from Video Demonstrations [**IL**] [[paper](https://arxiv.org/abs/2501.14208)]

- [2024.12] AnyBimanual: Transferring Unimanual Policy for General Bimanual Manipulation [**RL**] [[paper](https://arxiv.org/abs/2412.06779)] [[project](https://manicm-fast.github.io/)] [[code](https://github.com/TengBoYuu/AnyBimanual)]

- [2024.11] AsymDex: Leveraging Asymmetry and Relative Motion in Learning Bimanual Dexterity [**RL**] [[paper](https://arxiv.org/abs/2411.13020)] [[project](https://sites.google.com/view/asymdex-2024/)]

- [2024.10] RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation [**IL**] [**foundation**] [[github](https://github.com/thu-ml/RoboticsDiffusionTransformer)] [[paper](https://arxiv.org/abs/2410.07864)] [[project](https://rdt-robotics.github.io/rdt-robotics/)]

- [2024.10] ALOHA Unleashed: A Simple Recipe for Robot Dexterity [**IL**] [[project](https://aloha-unleashed.github.io/)] [[paper](https://arxiv.org/abs/2410.13126)]

- [2024.09] ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation [**VLM**] [[project](https://rekep-robot.github.io/)] [[paper](https://rekep-robot.github.io/rekep.pdf)] [[code](https://github.com/huangwl18/ReKep)]

- [2024.07] VoxAct-B: Voxel-Based Acting and Stabilizing Policy for Bimanual Manipulation [**IL**] [**VLM**] [[project](https://github.com/VoxAct-B/voxactb)] [[paper](https://arxiv.org/abs/2407.04152)] [[code](https://github.com/VoxAct-B/voxactb)]

- [2024.07] PerAct2: Benchmarking and Learning for Robotic Bimanual Manipulation Tasks [**IL**] [[project](https://bimanual.github.io/)] [[paper](https://arxiv.org/abs/2407.00278)] [[code](https://github.com/markusgrotz/peract_bimanual)]

- [2024.01] Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation [**IL**] [[project](https://mobile-aloha.github.io/)] [[paper](http://arxiv.org/abs/2401.02117)] [[code(learning)](https://github.com/MarkFzp/act-plus-plus)] [[code(hardware)](https://github.com/MarkFzp/mobile-aloha)]


<a name="PhysicallySimulatedHumanoidAnimations" />

### Physically Simulated Humanoid Animations and Digital Human-Object Interaction

- [2025.11] SIMS: Simulating Human-Scene Interactions with Real World Script Planning [**RL**] [[paper](https://arxiv.org/abs/2411.19921)]

- [2025.02] InterMimic: Towards Universal Whole-Body Control for Physics-Based Human-Object Interactions [**RL**] [[paper](https://arxiv.org/abs/2502.20390)]

- [2024.10] Autonomous Character-Scene Interaction Synthesis from Text Instruction [**mocap**] [[project](https://lingomotions.com/)] [[paper](https://arxiv.org/abs/2410.03187)]

- [2024.07] Grasping Diverse Objects with Simulated Humanoids [**RL**] [[project](https://www.zhengyiluo.com/Omnigrasp-Site/)] [[paper](https://arxiv.org/abs/2407.11385)]

- [2024.06] Human-Object Interaction from Human-Level Instructions [**LLM**] [[project](https://hoifhli.github.io/)] [[paper](https://arxiv.org/abs/2406.17840)]

- [2024.06] CooHOI: Learning Cooperative Human-Object Interaction with Manipulated Object Dynamics [**RL**] [[project](https://gao-jiawei.com/Research/CooHOI/)] [[paper](https://arxiv.org/abs/2406.14558)]

- [2024.06] CORE4D: A 4D Human-Object-Human Interaction Dataset for Collaborative Object REarrangement [**mocap**] [[project](https://core4d.github.io/)] [[paper](https://arxiv.org/abs/2406.19353)] [[code](https://github.com/leolyliu/CORE4D-Instructions)]

- [2024.04] HOI-M3: Capture Multiple Humans and Objects Interaction within Contextual Environment [**mocap**] [[project](https://juzezhang.github.io/HOIM3_ProjectPage/)] [[paper](https://arxiv.org/abs/2404.00299)] [[code](https://github.com/Juzezhang/NeuralDome_Toolbox)]

- [2024.03] AnySkill: Learning Open-Vocabulary Physical Skill for Interactive Agents [**RL**] [[project](https://anyskill.github.io/)] [[paper](https://arxiv.org/abs/2403.12835)] [[code](https://github.com/jiemingcui/anyskill)]
