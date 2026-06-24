# FT-WBC Project Website

This repository contains the project website for **FT-WBC: Learning Fault-Tolerant Whole-Body Control for Legged Loco-Manipulation**.

FT-WBC is a fault-tolerant loco-manipulation framework for legged robots under lower-limb actuator failures. The website presents the paper, method overview, simulation and real-world demonstrations, code link, and citation information.

## Project Overview

Legged manipulators combine the mobility of quadruped platforms with the manipulation capability of robotic arms. However, arm-induced center-of-mass shifts and dynamic disturbances make the whole system more vulnerable to actuator failures, which can cause falls, object drops, and task failures.

FT-WBC improves robustness under actuator weakening and locked-joint failures through:

- a decoupled upper-body and lower-body policy architecture;
- a **Fault Estimator (FE)** that predicts faulty joints from proprioceptive histories;
- a **Posture Adaptation Module (PAM)** that maps manipulation-driven base posture plans into safe executable posture commands;
- fault-aware posture adaptation for compensatory gaits, stable whole-body control, and preserved arm workspace.

Simulation and real-world experiments are conducted on a Unitree Go2 equipped with an Airbot Play arm, showing improved survival rate and reachable workspace under actuator failures with zero-shot transfer to the real robot.

## Website Content

The website includes the following sections:

- **Title and Authors**: Project title, author list, and affiliations.
- **Paper / arXiv / Code Links**: Direct links to the paper, arXiv page, and GitHub repository.
- **Baseline Failure Videos**: Examples showing that nominal locomotion and whole-body policies fail under actuator faults.
- **Abstract**: Summary of the motivation, method, and experimental findings.
- **Overview Video**: Main video introduction for FT-WBC.
- **Framework Overview**: Diagram and description of the FE, PAM, leg policy, and arm policy pipeline.
- **Real-World Demonstrations**: Videos for weakening faults and locked faults across locomotion, whole-body control, and pick-and-place tasks.
- **BibTeX**: Citation entry for the project.

## Resources

- Paper: `./static/pdfs/example.pdf`
- arXiv: <http://arxiv.org/abs/2606.24466>
- Code: <https://github.com/hhhappyshow/FT-WBC-Learning-Fault-Tolerant-Whole-Body-Control-for-Legged-Loco-Manipulation>

## Local Development

To preview the website locally, serve this directory with a simple HTTP server and open the local address in a browser.

For example, from this folder:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Citation

If you find this work useful, please cite:

```bibtex
@article{zhong2026ftwbc,
  title   = {FT-WBC: Learning Fault-Tolerant Whole-Body Control for Legged Loco-Manipulation},
  author  = {Yudong Zhong and Pengfei Mai and Sikai Guo and Jiahang Cao and Zhihai Bi and Qiuyue Liu and Ziyan Feng and Jinni Zhou and Jun Ma},
  journal = {arXiv preprint arXiv:2606.24466},
  year    = {2026},
}
```

## Acknowledgement

This project page is adapted from the [Nerfies website template](https://nerfies.github.io).

## Website License

The website template follows the Creative Commons Attribution-ShareAlike 4.0 International License. Please also respect the licenses of the project materials, videos, figures, and third-party assets used in this repository.