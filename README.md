<!--
  ════════════════════════════════════════════════════════════════
  HOSSAM (@SamDozer) — GITHUB PROFILE README
  Only remaining placeholder:
    #LINKEDIN#  → your LinkedIn URL (appears twice)
  Everything else is filled in and live.
  This README is fully self-contained — no image files to upload.
  ════════════════════════════════════════════════════════════════
-->

<!-- ===================== TYPING BANNER ===================== -->
<div align="center">

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=6366F1&center=true&vCenter=true&width=720&height=60&lines=Computational+Biologist+%F0%9F%A7%AC;Molecular+Dynamics+%26+Simulation;Curious+about+Neuroscience+%F0%9F%A7%A0;Guitarist+who+ships+apps+%F0%9F%8E%B8;Reproducible+science%2C+always" alt="Typing SVG" />

</div>

<!-- ===================== SOCIAL BADGES ===================== -->
<div align="center">

  <a href="#LINKEDIN#"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:hossam.mahmoud12@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/SamDozer?tab=repositories"><img src="https://img.shields.io/badge/Open_Source-MIT-A6CE39?style=for-the-badge&logo=opensourceinitiative&logoColor=white" alt="Open Source"/></a>
  <br/>
  <img src="https://komarev.com/ghpvc/?username=SamDozer&label=Profile%20Views&color=6366F1&style=for-the-badge&abbreviated=true" alt="Profile views"/>
  <a href="https://github.com/SamDozer?tab=followers"><img src="https://img.shields.io/github/followers/SamDozer?label=Follow&style=social" alt="Followers"/></a>

</div>

<!-- ===================== ABOUT ME ===================== -->
## 🧬 About Me

I'm a **computational biologist** at **Cairo University** who builds the tooling that makes computational science reproducible. Most of my work turns a messy simulation directory into something a reader can actually trust: automated analysis, publication-quality figures, and a provenance record of exactly how every number was produced.

I also play **guitar** — and my favourite project is the one where those two worlds collide.

```yaml
name:      Hossam
role:      Computational Biologist  ·  Simulation & Scientific Tooling
based in:  Cairo, Egypt  ·  Cairo University
works on:  GROMACS molecular dynamics · tumor growth modeling · reproducible pipelines
curious:   computational neuroscience · structural biophysics
also:      Flutter apps for guitarists  🎸
principle: "If it isn't reproducible, it isn't a result"
```

- 🔬 Building **[mdforge](https://github.com/SamDozer/molecular-dynamics-forge)** — one command from raw GROMACS output to a full, reproducible analysis
- 🎸 Shipping **[exercio](https://github.com/SamDozer/exercio)** — an offline-first guitar practice app, currently in public beta
- 🧠 Drawn to **computational neuroscience** — modeling the brain is the problem I most want to work on next
- 🔭 Also interested in **structural biophysics, biological modeling, and open reproducible science**
- 📫 Reach me at **hossam.mahmoud12@gmail.com**

<!-- ===================== FLAGSHIP: EXERCIO ===================== -->
## 🎸 Flagship Project — Exercio

> ### [**exercio**](https://github.com/SamDozer/exercio) — offline-first guitar practice, routine building & progress tracking
>
> Most practice sessions have no structure. Exercio gives them **sections with targets, exercises with tempos, and an honest record of what actually happened.**

The project I'm proudest of — my two obsessions, guitar and rigorous engineering, in one Android app.

**What it does**
- 🧬 **Guitar DNA** — an 8-question profile generates a personalized routine through a *fully deterministic, on-device* algorithm. Same answers, same routine, every time. No randomness, no network calls.
- ⏱️ **Practice mode** — section and per-exercise focus timers. Overrunning a target is *recorded, not blocked* — the app learns from what you really did.
- 🥁 **Metronome** — 6 synthesized sound packs, hold-to-sweep tempo, running as an Android foreground service so it survives a locked screen.
- 📈 **Progress tracking** — per-attempt tempo, quality, fatigue and tuning logs, with clean-streak and tempo-progress analytics that recompute retroactively.
- 📚 **147 practice topics** across 15 categories — all stored as *data*, never hard-coded screens.
- 🎨 **6 themes** — a token-based design system where a theme changes colors, typography, animation **and the metronome's voice** without touching feature code.

**Engineering worth a look**
- **Layered pub workspace:** `practice_core` is pure Dart with *zero* external dependencies — no Flutter, no database, no platform code — with the dependency rule enforced by a **CI-run architecture checker**.
- **Privacy by construction:** no accounts, no analytics SDKs, no crash reporting, no uploads. Everything stays on the phone.
- Native **Kotlin** audio engine behind a Dart API contract.

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![SQLite](https://img.shields.io/badge/Drift_·_SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

<a href="https://github.com/SamDozer/exercio"><img src="https://img.shields.io/badge/v0.1.0--beta.1-public_beta-6366F1?style=for-the-badge" alt="beta"/></a>
<a href="https://github.com/SamDozer/exercio"><img src="https://img.shields.io/badge/License-MIT-A6CE39?style=for-the-badge" alt="MIT"/></a>

</div>

<!-- ===================== RESEARCH ===================== -->
## 🔬 Research & Scientific Tooling

### 🧪 [molecular-dynamics-forge (`mdforge`)](https://github.com/SamDozer/molecular-dynamics-forge)
> *"Turns a GROMACS simulation directory into a complete, publication-quality, fully reproducible analysis — with minimal input."*

Auto-detects system composition, picks the right analyses, and runs **24 built-in analyses** — RMSD, Rg, SASA, H-bonds, RMSF, DSSP, PCA, clustering, salt bridges, contact maps, native contacts, interface and binding-pocket analysis. Every run writes a **manifest** recording library versions, git commit, input fingerprints, parameters and runtimes. Plugin architecture for custom analyses; config-driven for batch/HPC; containerized for a reproducible environment.

`Python 3.10+` `MDAnalysis` `MDTraj` `GROMACS` `Docker`

### 🧬 [alpha-zein-md-analysis](https://github.com/SamDozer/alpha-zein-md-analysis)
A publication-quality pipeline for a **100 ns CHARMM36 simulation of α-zein** (UniProt A8HNE1, 187 residues) built from an **AlphaFold 3** model. 20+ self-contained analyses — RMSD with moving-average plateau detection, RMSF, Rg, SASA, H-bond networks, PCA + free-energy landscapes, DCCM, DSSP, native contacts, clustering, residue interaction networks. Trajectories are preprocessed once into a lean protein-only file for fast downstream runs; outputs are 300 DPI PNG + PDF figures, CSV datasets and an auto-generated interpretive report.

`Python` `MDAnalysis` `MDTraj` `panedr` `AlphaFold 3`

### 📊 [2D-Tumor-Angiogenesis-Simulation](https://github.com/SamDozer/2D-Tumor-Angiogenesis-Simulation)
Five progressive notebooks modeling tumor growth as coupled **diffusion, logistic proliferation and angiogenesis**. Solves the **Fisher–Kolmogorov PDE** by finite differences with a 5-point Laplacian stencil on grids up to 200×200, sweeping diffusion coefficients, proliferation rates and vessel capacity — ending in a fully coupled tumor–vasculature field where vessels adapt to nutrient demand.

`Python` `NumPy` `Matplotlib` `Jupyter`

<!-- ===================== LEARNING TOOLS ===================== -->
## 🎓 Learning Tools

### 📝 [ExamForge](https://github.com/SamDozer/Exam-Forge) · [exam-study-guide-predictor](https://github.com/SamDozer/exam-study-guide-predictor)
> *"Predict the paper → forge the study guide → drill it to retention."*

Turns lecture slides, past papers, lab manuals and professor transcripts (**English or Arabic**) into source-grounded study guides, **confidence-tagged** exam predictions and spaced-repetition drills. Evidence is explicitly weighted — past papers strongest, textbook mentions weakest — and AI-inferred predictions are visibly separated from what a professor actually said. Ships as both a Claude chat skill and a Claude Code kit with persistent progress tracking.

`Python` `Claude Skills` `Spaced Repetition`

<!-- ===================== TECH STACK ===================== -->
## 🧰 Toolkit

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=sqlite&logoColor=white)

**Scientific Python**

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

**Molecular Dynamics & Structural Biology**

![GROMACS](https://img.shields.io/badge/GROMACS-1F6FEB?style=for-the-badge&logoColor=white)
![MDAnalysis](https://img.shields.io/badge/MDAnalysis-E97627?style=for-the-badge&logoColor=white)
![MDTraj](https://img.shields.io/badge/MDTraj-2E7D32?style=for-the-badge&logoColor=white)
![CHARMM36](https://img.shields.io/badge/CHARMM36-6A1B9A?style=for-the-badge&logoColor=white)
![AlphaFold](https://img.shields.io/badge/AlphaFold_3-8B5CF6?style=for-the-badge&logoColor=white)

**Mobile & Tooling**

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

<!-- ===================== GITHUB ANALYTICS ===================== -->
## 📊 GitHub Analytics

<!--
  NOTE: the two github-readme-stats cards below use a shared public instance
  that is frequently over quota and returns 503 (it was down when this was
  written). The URLs are correct — if the cards show broken, that's upstream.
  Permanent fix: deploy your own instance (free) and swap the hostname:
  https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own-vercel-instance
-->
<div align="center">

  <img height="165" src="https://github-readme-stats.vercel.app/api?username=SamDozer&show_icons=true&count_private=true&hide_border=true&theme=tokyonight" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SamDozer&layout=compact&langs_count=8&hide_border=true&theme=tokyonight" alt="Top languages"/>

  <br/><br/>

  <img src="https://github-readme-streak-stats.herokuapp.com/?user=SamDozer&hide_border=true&theme=tokyonight" alt="GitHub streak"/>

  <br/><br/>

  <img src="https://github-readme-activity-graph.vercel.app/graph?username=SamDozer&theme=react-dark&hide_border=true&area=true" alt="Activity graph"/>

</div>

<!-- ===================== SNAKE ANIMATION ===================== -->
<!--
  Needs .github/workflows/snake.yml to run once (Actions tab → run it),
  then delete the comment markers around the block below.
-->
<!--
<div align="center">
  <img src="https://raw.githubusercontent.com/SamDozer/SamDozer/output/github-contribution-grid-snake-dark.svg" alt="Snake animation"/>
</div>
-->

<!-- ===================== BEYOND THE CODE ===================== -->
## 🌙 Beyond the Code

Between simulation runs, I'm usually on the guitar — which is exactly how [exercio](https://github.com/SamDozer/exercio) got written. A good solo and a good pipeline are built the same way: patient iteration until it's right.

<div align="center">
  <br/>
  <em>A brutally honest look at my focus levels between experiments 👇</em>
  <br/><br/>
  <img src="https://user-images.githubusercontent.com/74038190/212284094-e50ceae2-de86-4dd6-9f9c-a3ebcb3ede9e.gif" width="360" alt="Unproductive all day"/>
</div>

<!-- ===================== FREE SOFTWARE ===================== -->
## 🕊️ Free Software & Open Source

I'm a firm believer in **free and open source software** — it's the reason I adore GitHub and platforms like it. Knowledge that can be read, copied, corrected and built upon is knowledge that survives. That belief isn't decorative: **every public repository I own is MIT licensed**, and [exercio](https://github.com/SamDozer/exercio) is free software down to its fonts.

Science and free software want the same thing. A result you can't reproduce isn't a result; a program you can't read isn't knowledge. Both only work when people are allowed to look inside.

> ### *"My work on free software is motivated by an idealistic goal: spreading freedom and cooperation."*
>
> — **Richard Stallman**
<div align="center">

![Open Source](https://img.shields.io/badge/Open_Source-Believer-A6CE39?style=for-the-badge&logo=opensourceinitiative&logoColor=white)
![MIT](https://img.shields.io/badge/All_My_Repos-MIT-6366F1?style=for-the-badge&logo=github&logoColor=white)
![GNU](https://img.shields.io/badge/Free_Software-GNU-8B5CF6?style=for-the-badge&logo=gnu&logoColor=white)

</div>

<!-- ===================== CONNECT ===================== -->
## 📫 Let's Connect

<div align="center">

  <a href="#LINKEDIN#"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:hossam.mahmoud12@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/SamDozer"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>

  <br/><br/>
  <i>"If it isn't reproducible, it isn't a result."</i>

</div>

<!-- ===================== FOOTER WAVE ===================== -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6366F1,8B5CF6,A6CE39&height=100&section=footer" width="100%" alt="footer wave"/>
</div>
