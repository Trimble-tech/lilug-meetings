# Febuary 2025 LILUG Meeting
*Febuary 11th, 2025 @ [Digital Ballpark](https://maps.app.goo.gl/Uef2PiZBpZLd1n3QA)*
*Pace-notes by [Chris Trimble](https://github.com/Trimble-tech)*

## News & Small Talk
- Nothing this month

## Main Discussion: Sokoly Computerized Automated Lethal Munitions
*By Yutong Zhang & Fang Luo*

**This is a discussion on automated weapons and the current status of AI in drone warfare. Sokoly Systems is a Ukrainian weapons manufacturer which is studied in this discussion. The presenters are not affiliated with Sokoly Systems. Sokoly Systems can be found here: <https://sokolysystems.com>**

### Introduction
- Drones are reshaping warfare
- Cost advantage of drones is present

#### Challenges of drones:
- Operator Training
- Electronic Countermeasures
- Manufacturing & Supply Chain Issues
- Noise from drones cab ne hard when flying lower than 100 meters
- Swarms of other drones can be set to target and impact into drones

#### Feasibility of AI Hardware in Drones
- AI from ARM or RISC-V hobby boards (such as Rockchip, Raspberry PI, etc.) is being fitted to certain drones to advance aiming abilities.
- Once operation is autonomous, jamming will not work as commands are done locally

**Possible uses of Machine Learning/AI in warfare**
- Semi-Auto operation
- tracking & aiming with visual and thermal cameras

### Examination of Sokoly Systems SAMURAI Visual Object Tracker
**Tracking Process:**
1. Raw Sequence
2. Image
3. Encoder
4. Memory Attention
5. Mask Decoder
6. Affinity to head/object head
7. Affinity score & object scores
8. Memory Bank
9. Memory Selection
10. Motion-aware instance-level memory
11. Feedback to memory attention

- This process shows how the system can learn and improve judgement as data develops.
- Redefining model and reducing noise is critical: 0.005% noise can change the image detection greatly; this highlights potential trust issues and accuracy issuses of AI image detection.

### Training & Refinement of AI/Machine Learning Models for Drone Use Case
- Enforcement/guidance of AI mode4ls can be manually coded or automatically guided by coded functions.
- Visual object trackers like SAMURAI can support other systems like SAM2 (real-time footage from existing weapons systems).
- Model can be trained within simulated environments; Unreal Engine is one tool used to digitally simulate training.

**Optical Flow-Real Projective Geometry + IMU Dynamics Algorithm**
- Enables natural, highly manuverable autonomous tracking with visual footage/video.
- Terminal guidance requires no operator intervention and is resistant to electromagnetic interference.
- Can go without some sensors (less accelerometers & gyroscopes) as the model can determine horizon level and inertia.
Avoinics equipment can be used as control analogy for drones; sensors, radios, and control units can be shrunk from a full plane to one circuit board.
VLM (Visual Language Modelling) can be used to train models. By feeding individual images into the model and tuning outputs from it more refined action can be dictated. An example is learning when an individual has surrendered.

### Presenter Take-Away & Developments
- Developing data models and hardware prototypes can be done academically to explore the evolution of this technology.
- Expanding use cases and understanding hardware needs of AI/machine learning for drones.
- Management of weapons systems or surveillance computers can be made easier for higher precision.

### Secretary Take-Away
***War sucks***, and autonomous warfare is a scary development.
However, we can analyze tech like this to better understand *good* uses of AI or machine learning.

When the hatchet is buried we can focus on:
- Semi-autonomous driving
- Image detection for cameras
- Medical imaging (detecting things like tumors in sensors/cameras)
- Home security (how about a camera to tell occupants when you came home?)