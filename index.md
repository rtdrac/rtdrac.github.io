---
title: Welcome!
layout: home
part: ' '
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---

# Real-Time Drum Accompaniment Systems (RT-DR-AC)
{: .fs-9 }

{: .fs-7}
All supplementary material for the following thesis manuscript can be found here 

---
## Dissertation Download
{: .fs-9 }

<br>

[Download Dissertation](https://drive.google.com/file/d/1YWjblx6cmUo-wYV2ECZAOS1S3zUHBOn1/view){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

---

## Abstract
{: .fs-9 }

<br>

This dissertation examines the generation of real-time symbolic drum accompaniments, with a particular focus on live improvisation contexts. While the research does occasionally focus on the audio domain, the majority of the research is centered on symbolic-to-symbolic systems. This dissertation addresses real-time drum accompaniment from multiple perspectives: (1) conceptual, where a target application is designed based on a set of specified requirements, (2) architectural, where specific generative models are designed and developed for the selected conceptual design, and (3) deployment, where the conceptual design is realized and evaluated. Throughout this work, three accompaniment systems were developed and refined.

The first work, detailed in Chapters 3 and 4, was aimed to develop a light-weight system on which future more sophisticated designs could be based. This system was based on a transformer model that was developed to convert a monotonic (single voice) rhythmic loop (groove) into a full multi-voice drum loop. The concept explored here was to investigate whether a loop-based system could be effectively used for generating drum accompaniments in long evolving improvisational sessions. The resulting system was evaluated by professional musician Raül Refree, who provided valuable insights on how the design could be modified to better suit the task.

Following these evaluations, the second system, GrooveTransformer, was developed (discussed in Chapter 5). In this work, rather than relying on our personal speculations, we collaborated with Refree from the outset of the project. As such, we were able to develop a system that was far more suitable for the task at hand, to the extent that the musician felt comfortable to perform with the system in a public live improvisational session. While still loop-based, the generative model in this work was based on a variational transformer that enabled us to address the majority of the collaborating musician's requirements for the system. Although initially deployed as software, we also developed a hardware Eurorack version (discussed in Chapter 6). The Eurorack module was designed to encourage experimentation and exploration beyond the system's original intent. 

In the third system (discussed in Chapter 7), we moved beyond the loop-based approach. The primary goal was to enhance the system's awareness of the evolving performance over extended durations. To this end, we developed a new generative model with a much larger context. The larger model's computational demands required a thorough exploration of both conceptual and technical deployment strategies.

All of these systems focused on converting a monotonic groove into a multi-voice drum pattern. In Chapter 8, we first discuss the limitations and affordances of basing the generations solely on groove. Additionally, several works and proposals surrounding this groove-to-drum approach are discussed in detail: (1) how to improve the process of extracting grooves from polyphonic sources, (2) how to make this approach more accommodating for individuals with varying levels of musical experience, (3) how to expand the concept to generate general rhythms rather than exclusively drums, and (4) how to extract groove from audio sources.

Beyond the primary objectives, this research also yielded several significant secondary contributions that arose from the explorations conducted. One such achievement was that we were able to establish that our systems can also be adapted to work with audios without major architectural changes (Appendix A). Moreover, we created NeuralMidiFx (Appendix B), a wrapper designed to facilitate the deployment of neural networks in VST (Virtual Studio Technology) format. This tool was developed to overcome the technical challenges encountered during the real-time deployment of the generative models. Furthermore, two novel datasets, TapTamDrum (Appendix C) and El Bongosero (Appendix D), were created as part of this research. These datasets serve as valuable resources for future studies on both rhythm generation and rhythm analysis.

