# An Orchestration Framework for Open System Models of Reconfigurable Intelligent Surfaces

This is a research-oriented code package that is primarily intended to allow readers to replicate the results of the article mentioned below and also encourage and accelerate further research on this topic:

V. Croisfelt, F. Devoti, F. Saggese, V. Sciancalepore, X. Costa-Pérez and P. Popovski, "Autonomous RISs and Oblivious Base Stations: The Observer Effect and Its Mitigation," in IEEE Transactions on Wireless Communications, vol. 24, no. 6, pp. 5129-5145, June 2025, doi: 10.1109/TWC.2025.3546118.

A pre-print version is available on arXiv: https://arxiv.org/abs/2304.10858.

We hope this content helps in your research and contributes to building the precepts behind open science. Remarkably, to boost the idea of open science and further drive the evolution of science, I also motivate you to share your published results with the public.

If you have any questions or if you have encountered any inconsistency, please do not hesitate to contact me via victorcroisfelt@gmail.com.

## Abstract
To obviate the control of reflective intelligent surfaces (RISs) and the related control overhead, recent works envisioned autonomous and self-configuring RISs that do not need explicit use of control channels. Instead, these devices, named hybrid RISs (HRISs), are equipped with receiving radio-frequency (RF) chains and can perform sensing operations to act independently and in parallel to the other network entities. A natural problem then emerges: as the HRIS operates concurrently with the communication protocols, how should its operation modes be scheduled in time such that it helps the network while minimizing any undesirable effects? In this paper, we propose an orchestration framework that answers this question, revealing an engineering trade-off, called the self-configuring trade-off, that characterizes the applicability of self-configuring HRISs under the consideration of massive multiple-input multiple-output (mMIMO) networks. We evaluate our proposed framework considering two different HRIS hardware architectures, the power- and signal-based HRISs that differ in their hardware complexity. The numerical results show that the self-configuring HRIS can offer significant performance gains when adopting our framework. 

## Content
The code provided here can be used to simulate Figs. 6 and 7 of the paper. The code is organized in the following way:
  - sim_figureX.py: simulation scripts that store the data points needed to plot each figure as a .npz file in /data folder.
  - /data: here you can find the .npz files output by each simulation script. NOTE: You should run the simulation scripts by yourself, since the files are too large to share using GitHub.
  - plot_figureX: scripts to plot each one of the figures by loading the .npz files. The output of this script is the corresponding figure in TikZ.
  - /src: define classes and functions needed to run the simulations.
  - /tikz: where the .tex's of the figures are saved.

## Citing this Repository and License
This code is subject to the MIT license. If you use any part of this repository for research, please consider citing our aforementioned work.

```bibtex
@ARTICLE{10914507,
  author={Croisfelt, Victor and Devoti, Francesco and Saggese, Fabio and Sciancalepore, Vincenzo and Costa-Pérez, Xavier and Popovski, Petar},
  journal={IEEE Transactions on Wireless Communications}, 
  title={Autonomous RISs and Oblivious Base Stations: The Observer Effect and Its Mitigation}, 
  year={2025},
  volume={24},
  number={6},
  pages={5129-5145},
  keywords={Probes;Distortion;Human-robot interaction;Hardware;Complexity theory;Reconfigurable intelligent surfaces;Vectors;Remote control;Reflection;Real-time systems;Reconfigurable intelligent surface (RIS);intelligent reflective surface (IRS);hybrid reconfigurable intelligent surface (HRIS);massive multiple-input multiple-output (MIMO)},
  doi={10.1109/TWC.2025.3546118}}
```

## Acknowledgement
This work was supported by the Villum Investigator Grant “WATER” from the Villum Fonden, Denmark.
