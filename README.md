<h1 align="center">Ashutosh Kumar Singh</h1>

<h3 align="center">Security Engineer @ Skyhigh Security · ML Systems Researcher · NeurIPS 2026 Author</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/ashutosh-kumar-singh951/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:ashutoshkumarsingh951@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white" />
  </a>
  <a href="https://ashutosh-kumar-singh.vercel.app">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white" />
  </a>
  <a href="https://medium.com/@ashutoshkumars1ngh">
    <img src="https://img.shields.io/badge/Blog-12100E?style=flat&logo=medium&logoColor=white" />
  </a>
</p>

---

### 🔬 What I Do

I build secure, scalable systems at **Skyhigh Security** and contribute to the reliability of production ML infrastructure across Apple, Google, and OpenAI. My current research focus is **numerical stability in half-precision inference** on neural accelerators — work that led to a **NeurIPS 2026 workshop paper submission** and fixes deployed across Apple's entire ML compiler stack.

---

### 🍎 Featured: Apple ML Framework Contributions

> **4 PRs · 6 Issues · 3 Apple repos · 21 production models protected**

I discovered a systematic class of **fp16 overflow failures** on Apple Neural Engine that silently produce incorrect outputs in operations like `softplus`, `mish`, and `logsumexp`. I derived mathematically equivalent, overflow-proof decompositions and submitted fixes across Apple's ML stack:

| Repository | Contribution | Status |
|:-----------|:-------------|:-------|
| [apple/coremltools](https://github.com/apple/coremltools/pull/2725) | PRs [#2725](https://github.com/apple/coremltools/pull/2725), [#2726](https://github.com/apple/coremltools/pull/2726), [#2727](https://github.com/apple/coremltools/pull/2727) — Stable decompositions for 5 ops | ✅ **Approved & merge-ready** |
| [apple/coreai-torch](https://github.com/apple/coreai-torch/pull/22) | PR [#22](https://github.com/apple/coreai-torch/pull/22) — First external fp16 fix on WWDC 2026 framework | 🟡 Under review |
| [apple/coreai-optimization](https://github.com/apple/coreai-optimization/issues/7) | Issue [#7](https://github.com/apple/coreai-optimization/issues/7) — FP16 casting × quantization compound vulnerability | 🟡 Reported |

**Impact:** Fixes protect all 21 Core AI production model recipes (Gemma3, Qwen3, Mistral, Whisper, YOLO, SAM3, Stable Diffusion, etc.) from silent numerical failures on 2.5B+ Apple Silicon devices.

---

### 🏆 Open-Source Track Record

<p align="left">
  <a href="https://github.com/apple/coremltools/pull/2725">
    <img src="https://img.shields.io/badge/Contributor-Apple%20coremltools-000000?style=for-the-badge&logo=apple&logoColor=white" />
  </a>
  <a href="https://github.com/apple/coreai-torch/pull/22">
    <img src="https://img.shields.io/badge/Contributor-Apple%20Core%20AI-000000?style=for-the-badge&logo=apple&logoColor=white" />
  </a>
  <a href="https://github.com/google-deepmind/chex/pull/423#pullrequestreview-3631540580">
    <img src="https://img.shields.io/badge/Contributor-Google%20DeepMind-4285F4?style=for-the-badge&logo=google&logoColor=white" />
  </a>
  <a href="https://github.com/openai/codex/pull/10729">
    <img src="https://img.shields.io/badge/Contributor-OpenAI%20Codex-000000?style=for-the-badge&logo=openai&logoColor=white" />
  </a>
  <a href="https://github.com/tenstorrent/tt-metal/issues/31286#issuecomment-4503856597">
    <img src="https://img.shields.io/badge/Bounty%20%241%2C500-Tenstorrent-7B2FF7?style=for-the-badge" />
  </a>
  <a href="https://github.com/tensorflow/tensorflow/pull/120175">
    <img src="https://img.shields.io/badge/Security-TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  </a>
  <a href="https://github.com/google/adk-python/pull/5927">
    <img src="https://img.shields.io/badge/Security-Google%20ADK-EA4335?style=for-the-badge&logo=google&logoColor=white" />
  </a>
  <a href="https://github.com/bazelbuild/bazel/pull/28459">
    <img src="https://img.shields.io/badge/Contributor-Bazel-00ADEE?style=for-the-badge&logo=bazel&logoColor=white" />
  </a>
  <a href="https://github.com/stripe/stripe-js/issues/849#event-22146631473">
    <img src="https://img.shields.io/badge/Contributor-Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white" />
  </a>
</p>

| Project | What I Did | Impact |
|:--------|:-----------|:-------|
| **Google DeepMind** (Chex) | Modernized JAX sharding detection for JAX 0.8.x | Merged by DeepMind maintainer |
| **OpenAI Codex** | Fixed critical Windows TUI authentication bug | Merged into official repo |
| **Tenstorrent** ($1,500 bounty) | Ported Depth Anything V2 Large to TTNN (Wormhole B0) | PCC 0.9983, bounty completed |
| **Google ADK-Python** | Fixed path traversal / Zip Slip vulnerability (CWE-22) | Merged — prevented RCE |
| **TensorFlow** | Fixed 3 memory safety vulns (heap OOB, corruption, CHECK failures) | Merged — prevented crashes in prod ML |
| **Bazel** | Implemented TLS error fail-over in Repository Downloader | Merged into official repo |
| **Stripe** | Issue investigation and resolution in StripeJS | Resolved |

---

### 📄 Research

**[Compiler-Level Numerical Stabilization for Half-Precision Inference on Neural Accelerators](https://github.com/Ashutosh0x/fp16-numerical-stability-neurips2026)**
*NeurIPS 2026 Workshop Submission · Ashutosh Kumar Singh*

[![Read Paper](https://img.shields.io/badge/📄_Read_Full_Paper-LaTeX-blue?style=for-the-badge)](https://github.com/Ashutosh0x/fp16-numerical-stability-neurips2026)

Cross-framework audit of Apple's entire ML stack (5 frameworks × 5 operations × 21 models). Derived overflow-free algebraic decompositions validated on M3 Max and M5 silicon with zero regressions.

---

### 🛠 Tech Stack

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python" />
  <img width="8" />
  <img src="https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white&style=for-the-badge" height="30" alt="cplusplus" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original.svg" height="30" alt="go" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" height="30" alt="java" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="30" alt="react" />
  <img width="8" />
  <img src="https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white&style=for-the-badge" height="30" alt="nextjs" />
</div>

<div align="left">
  <img src="https://skillicons.dev/icons?i=aws" height="35" alt="aws" />
  <img width="8" />
  <img src="https://skillicons.dev/icons?i=gcp" height="35" alt="gcp" />
  <img width="8" />
  <img src="https://skillicons.dev/icons?i=azure" height="35" alt="azure" />
  <img width="8" />
  <img src="https://skillicons.dev/icons?i=docker" height="35" alt="docker" />
  <img width="8" />
  <img src="https://skillicons.dev/icons?i=kubernetes" height="35" alt="kubernetes" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/terraform/terraform-original.svg" height="35" alt="terraform" />
  <img width="8" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" height="35" alt="tensorflow" />
  <img width="8" />
  <img src="https://cdn.simpleicons.org/deepmind/4285F4" height="35" alt="deepmind" />
</div>

---

### 🎖️ Certifications

<table>
  <tr>
    <td align="center" width="120">
      <a href="https://www.credential.net/713ca820-7ced-43ef-baf0-4a4264806747" target="blank">
        <img src="https://images.credential.net/badge/tiny/zzteqp1f_1710821711216_badge.png" alt="Cloud Architect" height="80" width="80" />
      </a>
      <br /><sub><b>GCP Professional<br/>Cloud Architect</b></sub>
    </td>
    <td align="center" width="120">
      <a href="https://www.credential.net/713ca820-7ced-43ef-baf0-4a4264806747" target="blank">
        <img src="https://templates.images.credential.net/16590189116921664807425410566136.png" alt="Cloud Security" height="80" width="80" />
      </a>
      <br /><sub><b>GCP Cloud<br/>Security</b></sub>
    </td>
    <td align="center" width="120">
      <a href="https://www.credential.net/393ab745-c88d-4f7b-8115-481f0850c858" target="blank">
        <img src="https://images.credential.net/badge/tiny/2qo5o5vm_1710822118969_badge.png" alt="Cloud Digital Leader" height="80" width="80" />
      </a>
      <br /><sub><b>Cloud Digital<br/>Leader</b></sub>
    </td>
    <td align="center" width="120">
      <a href="https://www.credly.com/badges/890def21-59a7-43b7-8e2c-ba30dec236ab" target="blank">
        <img src="https://images.credly.com/images/be8fcaeb-c769-4858-b567-ffaaa73ce8cf/image.png" alt="Azure AZ-900" height="80" width="80" />
      </a>
      <br /><sub><b>Azure AZ-900</b></sub>
    </td>
    <td align="center" width="120">
      <a href="https://www.credly.com/earner/earned/badge/a465093d-9f50-4a81-a3a8-784ddaf2791e" target="blank">
        <img src="https://images.credly.com/images/fc1352af-87fa-4947-ba54-398a0e63322e/security-compliance-and-identity-fundamentals-600x600.png" alt="SC-900" height="80" width="80" />
      </a>
      <br /><sub><b>Microsoft SC-900</b></sub>
    </td>
    <td align="center" width="120">
      <a href="https://www.cloudskillsboost.google/public_profiles/9ee1d409-5342-4b96-bd6a-f7cc69bc82af" target="blank">
        <img src="https://github.com/Ashutosh0x/icons/blob/main/flycup%20challeneg.png" alt="GCP Fly Cup" height="80" width="80" />
      </a>
      <br /><sub><b>GCP Fly Cup</b></sub>
    </td>
    <td align="center" width="120">
      <a href="https://leetcode.com/u/Ashutosh0x/" target="blank">
        <img src="https://assets.leetcode.com/static_assets/others/2550.gif" alt="LeetCode 50 Days" height="80" width="80" />
      </a>
      <br /><sub><b>LeetCode 50</b></sub>
    </td>
  </tr>
</table>

---

### 📊 Stats

<div align="left">
  <img src="https://github-readme-stats-eight-theta.vercel.app/api?username=Ashutosh0x&show_icons=true&theme=radical&hide=contribs,issues&include_all_commits=true&count_private=true" height="150" alt="stats graph" />
  <img src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs?username=Ashutosh0x&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=6&theme=radical&hide_border=false" height="150" alt="languages graph" />
</div>

---

<p align="center">
  <b>Open to opportunities in ML Systems, Numerical Computing, and Infrastructure</b><br/>
  <a href="https://www.linkedin.com/in/ashutosh-kumar-singh951/">Let's connect →</a>
</p>

<img src="https://github.com/Ashutosh0x/icons/blob/main/snake.svg" alt="Snake animation" />
