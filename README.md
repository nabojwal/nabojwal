<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=24,20,17&height=140&section=header&text=Nabojwal%20Acharjee&fontSize=38&fontColor=D4AF37&animation=fadeIn&fontAlignY=55&desc=PhD%20Research%20Fellow%20%C2%B7%20IIT%20Madras&descSize=14&descAlignY=78&descColor=F5E6C8" width="100%"/>
</div>

<br/>

<div align="center">

*Inverse Problems · MRI Reconstruction · Deep Generative Models · Clinical AI*

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nabojwal-acharjee/)
&nbsp;
[![Email](https://img.shields.io/badge/mail-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nabojwal@gmail.com)
&nbsp;
[![Google Scholar](https://img.shields.io/badge/Scholar-4285F4?style=flat-square&logo=google-scholar&logoColor=white)](#)
&nbsp;
[![IIT Madras](https://img.shields.io/badge/IIT%20Madras-003087?style=flat-square)](https://www.iitm.ac.in)

</div>

<br/>

---

<br/>

## &nbsp; Research Mission

Medical imaging occupies an unusual position in science — it is one of the few fields where the quality of a mathematical reconstruction directly determines a clinical outcome. A poorly recovered MRI scan is not a failed benchmark; it is a missed diagnosis.

I work on the problem of **recovering diagnostic-quality images from severely undersampled MRI measurements** — using deep learning not as a black box, but as a structured prior that respects the physics of acquisition. My broader interest lies in understanding *when* learned reconstruction methods are trustworthy enough to use in practice, and *why* they fail when they do.

The questions that motivate me are not new. They are variants of problems that have been studied in signal processing, compressed sensing, and statistical estimation for decades. What is new is the set of tools we now have to approach them — and the responsibility that comes with deploying those tools in clinical settings.

<br/>

---

<br/>

## &nbsp; Research Focus

<details>
<summary><b>MRI Reconstruction & Accelerated Acquisition</b></summary>
<br/>

Acquiring a full MRI scan is slow. Undersampling k-space — the Fourier-domain measurements — dramatically reduces scan time, but recovery requires solving an ill-posed inverse problem. I develop deep learning architectures that are structurally aware of this problem: **unrolled optimization networks** that alternate between data consistency and learned regularization, and **diffusion model-based priors** that treat reconstruction as conditional sampling from a learned distribution over anatomical structure.

A recurring concern in my work is the gap between reconstruction quality on benchmark datasets (fastMRI, SKM-TEA) and performance on data collected with different scanners, field strengths, and acquisition protocols. Bridging that gap — through domain adaptation, physics-based invariances, or robust training strategies — is central to making these methods clinically deployable.

</details>

<details>
<summary><b>Generative Priors for Inverse Problems</b></summary>
<br/>

Score-based generative models and diffusion processes have opened a principled route to solving inverse problems in imaging: rather than learning a direct mapping from measurements to images, one learns a prior over the image distribution and then constrains sampling to be consistent with the observed measurements. This framing is mathematically elegant and practically powerful.

I am particularly interested in the theoretical underpinnings of this approach — conditions under which posterior sampling is well-posed, the effect of model misspecification on reconstruction fidelity, and whether the uncertainty captured by a diffusion posterior is meaningful in the clinical sense.

</details>

<details>
<summary><b>Uncertainty, Robustness & Clinical Realism</b></summary>
<br/>

A reconstruction algorithm that produces a confident output on every input is not necessarily a trustworthy one. Uncertainty quantification in deep learning for medical imaging remains genuinely hard — not because the methods are immature, but because calibration is difficult to define when ground truth is itself uncertain.

My work engages with this problem directly: how do we build systems that know when they are likely to fail? How do we test robustness not just to Gaussian noise perturbations, but to the real distribution shifts that occur in clinical deployment — equipment variation, patient motion, sequence parameter changes?

</details>

<br/>

---

<br/>

## &nbsp; Technical Ecosystem

**Languages & Scientific Computing**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Deep Learning & Numerical Methods**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![JAX](https://img.shields.io/badge/JAX-A8B9CC?style=flat-square&logo=google&logoColor=black)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white)

**Medical Imaging & MRI**

![MONAI](https://img.shields.io/badge/MONAI-1A73E8?style=flat-square)
![SimpleITK](https://img.shields.io/badge/SimpleITK-005571?style=flat-square)
![NiBabel](https://img.shields.io/badge/NiBabel-777BB4?style=flat-square)
![fastMRI](https://img.shields.io/badge/fastMRI-FF6B6B?style=flat-square)
![MRzero](https://img.shields.io/badge/MRzero-2d333b?style=flat-square)

**Infrastructure & Experiment Management**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Weights & Biases](https://img.shields.io/badge/W%26B-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

<br/>

---

<br/>

## &nbsp; Active Research Directions

> These are not projects in the conventional sense. They are active lines of inquiry — questions I am presently in the middle of answering.

<br/>

**`[I]` &nbsp; Physics-Informed Deep Unrolling for MRI Reconstruction**

Unrolled networks — architectures that unroll iterative optimization algorithms and replace hand-crafted priors with learned ones — occupy an interesting position between classical signal processing and modern deep learning. I am studying how to make these networks more robust to k-space sampling pattern variation and scanner heterogeneity, while preserving the interpretability that comes from their explicit algorithmic structure.

<br/>

**`[II]` &nbsp; Diffusion Posterior Sampling in k-Space**

Standard diffusion-based reconstruction methods operate in image space and enforce data consistency post-hoc. I am investigating formulations that work natively in the measurement domain — treating k-space itself as the space of observations and recovering images through constrained reverse diffusion. The theoretical and practical challenges here are non-trivial.

<br/>

**`[III]` &nbsp; Calibration & Uncertainty in Learned Reconstructions**

A reconstruction network's confidence score is only meaningful if it is calibrated against real failure modes. I am studying how to evaluate uncertainty in MRI reconstruction outputs — not by comparing to held-out test sets alone, but by examining behavior under clinically realistic perturbations that a model was never trained to handle.

<br/>

---

<br/>

## &nbsp; Publications & Manuscripts

<div align="center">

*Research output — full list on [Google Scholar](#)*

</div>

<br/>

<!-- Template for entries:
**Title of Paper**
Nabojwal Acharjee, Co-Author(s)
*Conference / Journal · Year*
[[PDF](#)] [[Code](#)] [[Poster](#)]
`keyword` `keyword`
-->

| | |
|---|---|
| **Status** | PhD research ongoing · manuscripts in preparation |
| **Topics** | MRI reconstruction · diffusion priors · uncertainty quantification |
| **Target venues** | MICCAI · NeurIPS · ISBI · Medical Image Analysis |

*I will populate this section as work reaches publication. I prefer to share results I stand behind over a high publication count.*

<br/>

---

<br/>

## &nbsp; GitHub

<div align="center">

<img height="155" src="https://github-readme-stats.vercel.app/api?username=nabojwal&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e&icon_color=3fb950&rank_icon=percentile&hide=prs,issues&include_all_commits=true" />
&nbsp;
<img height="155" src="https://github-readme-stats.vercel.app/api/top-langs/?username=nabojwal&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e&langs_count=5" />

</div>

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=nabojwal&bg_color=0d1117&color=3fb950&line=1f6feb&point=58a6ff&area_color=0d1117&area=true&hide_border=true&radius=4" width="92%"/>
</div>

<br/>

---

<br/>

## &nbsp; Collaboration

I am genuinely interested in working with people who take the following seriously:

- The **failure modes** of deep learning in safety-critical settings, not just benchmark performance
- The relationship between **mathematical structure** — compressed sensing, Bayesian inference, optimization theory — and what we observe empirically in trained networks
- **Clinical translation**: what it actually takes to move a reconstruction algorithm from a research paper into a hospital workflow

If your work touches any of these, I am open to conversation.

[![LinkedIn](https://img.shields.io/badge/Reach%20out%20on%20LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nabojwal-acharjee/)
&nbsp;
[![Email](https://img.shields.io/badge/Send%20an%20email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:nabojwal@gmail.com)

<br/>

---

<br/>

<div align="center">

<sub>

The hardest problems in medical imaging are not algorithmic.
They are epistemological: *how do we know when we can trust what we've recovered?*
That question is what keeps me working.

</sub>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=24,20,17&height=140&section=header&text=Nabojwal%20Acharjee&fontSize=38&fontColor=D4AF37&animation=fadeIn&fontAlignY=55&desc=PhD%20Research%20Fellow%20%C2%B7%20IIT%20Madras&descSize=14&descAlignY=78&descColor=F5E6C8" width="100%"/>

</div>
