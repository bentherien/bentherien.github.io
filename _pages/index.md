---
layout: page
title:
permalink: /
description: "Benjamin Thérien is a PhD student at Mila and Université de Montréal working on efficient LLM pre-training: distributed and communication-efficient optimization, learned optimizers, and continual pre-training. Previously at Google and Meta."
image: /images/avatar.jpg
---

<style>
/* Computer Modern (LaTeX), used for author lists and venues */
@font-face {
  font-family: "CMU Serif";
  font-style: normal;
  font-weight: 400;
  src: url("/fonts/cmu/cmu-serif-500-roman.woff2") format("woff2");
  font-display: swap;
}

@font-face {
  font-family: "CMU Serif";
  font-style: normal;
  font-weight: 700;
  src: url("/fonts/cmu/cmu-serif-700-roman.woff2") format("woff2");
  font-display: swap;
}

@font-face {
  font-family: "CMU Serif";
  font-style: italic;
  font-weight: 400;
  src: url("/fonts/cmu/cmu-serif-500-italic.woff2") format("woff2");
  font-display: swap;
}

@font-face {
  font-family: "CMU Serif";
  font-style: italic;
  font-weight: 700;
  src: url("/fonts/cmu/cmu-serif-700-italic.woff2") format("woff2");
  font-display: swap;
}

/* Calibri, falling back to Carlito (a metric-compatible open clone) where Calibri isn't installed */
/* Crisper text rendering */
body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}

body,
.site-name,
.site-description,
.page,
.page h1, .page h2, .page h3 {
  font-family: Calibri, Carlito, "Segoe UI", sans-serif !important;
}

:root {
  --accent: #1a62c0;
  --accent-dark: #1a5fb4;
  --accent-soft: #eaf2fd;
  --accent-border: #b9d2f3;
  --text: #2b2b2b;
  --muted: #666;
  --line: #e3e6ea;
}

.page {
  font-size: 18px;
  line-height: 1.7;
  color: var(--text);
}

.page a,
.about-section a {
  color: var(--accent);
}

/* Narrower column so lines stay readable */
.container {
  max-width: 960px !important;
  padding-left: 40px !important;
  padding-right: 40px !important;
}

/* Thin accent bar instead of the theme's black bar + rainbow strip */
#bar {
  display: none;
}

body:after {
  background: var(--accent) !important;
  height: 4px !important;
}

/* Header: photo on the left, name + bio + links on the right */
.masthead {
  padding-top: 36px !important;
  padding-bottom: 8px !important;
  border-bottom: none !important;
  display: flex;
  align-items: center; /* centre the photo vertically against the name + bio */
}

/* Left column: photo with the link icons underneath */
.avatar-col {
  flex: 0 0 280px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 18px;
  margin-right: 40px;
}

.site-avatar {
  width: 280px !important;
  height: 280px !important;
  float: none !important;
  margin: 0 !important;
}

.site-avatar img {
  width: 280px !important;
  height: 280px !important;
  border-radius: 12px !important;
}

.site-info {
  float: none !important;
  margin: 0 0 20px 0 !important;
  text-align: left !important;
  overflow: hidden !important; /* stay to the right of the photo */
}

.site-name {
  font-size: 38px !important;
  letter-spacing: normal !important;
  font-weight: bold !important;
  text-align: left !important;
  margin-bottom: 0 !important;
}

.site-name a {
  color: var(--text) !important;
}

.about-section {
  margin-top: 8px;
  font-size: 18px;
  line-height: 1.7;
  color: var(--text);
}

/* Icon links under the photo, in the link colour */
.social-icons {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 4px;
  float: none !important; /* undo the theme's nav float and margins */
  margin: 0 !important;
}

.social-icons a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 42px;
  height: 42px;
  margin: 0 !important;
  border-radius: 50%;
  color: var(--accent) !important;
  transition: background-color 0.15s, color 0.15s;
}

.social-icons a:hover,
.social-icons a:focus-visible {
  background-color: var(--accent-soft);
  color: var(--accent-dark) !important;
  text-decoration: none;
}

.social-icons svg {
  width: 24px;
  height: 24px;
  fill: currentColor;
}

/* Job-market banner */
.job-market {
  margin-top: 8px;
  padding: 20px 26px;
  border-radius: 12px;
  background: linear-gradient(135deg, var(--accent-dark), #1f6fd1);
  color: #fff;
  font-size: 18px;
  line-height: 1.6;
}

.job-market-title {
  font-size: 22px;
  font-weight: bold;
  margin-bottom: 2px;
}

.job-market {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: space-between;
  gap: 14px 24px;
}

.job-market-cta {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.job-market a.jm-btn {
  display: inline-block;
  padding: 6px 18px;
  border: 1.5px solid #fff;
  border-radius: 999px;
  background-color: #fff;
  color: var(--accent-dark) !important;
  font-size: 16px;
  font-weight: bold;
  text-decoration: none;
  transition: background-color 0.15s, color 0.15s;
}

.job-market a.jm-btn.ghost {
  background-color: transparent;
  color: #fff !important;
}

.job-market a.jm-btn:hover {
  background-color: var(--accent-soft);
  color: var(--accent-dark) !important;
}

/* Section heading */
.section-title {
  font-size: 28px !important;
  font-weight: bold !important;
  color: var(--text);
  margin: 44px 0 4px !important;
  padding-bottom: 6px;
  text-align: left !important;
  border-bottom: 2px solid var(--accent);
}

.section-sub {
  font-size: 16px;
  color: var(--muted);
  margin: 8px 0 4px;
}

/* Each paper is a card: fixed-size thumbnail frame + text */
.paper {
  display: flex;
  gap: 24px;
  align-items: flex-start;
  margin: 16px 0;
  padding: 18px 20px;
  border: 1px solid var(--line);
  border-radius: 12px;
  background-color: #fff;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
  transition: box-shadow 0.2s, border-color 0.2s;
}

.paper:hover {
  border-color: var(--accent-border);
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
}

.pub-thumb {
  flex: 0 0 220px;
  height: 140px;
  padding: 6px;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 8px;
  background-color: #f6f8fa;
}

.pub-thumb img {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}

.paper-body {
  flex: 1;
  min-width: 0;
}

.pub-title {
  font-size: 21px;
  font-weight: bold;
  line-height: 1.35;
  color: #1a1a1a;
  margin-bottom: 6px;
}

.pub-authors,
.pub-venue {
  font-family: "CMU Serif", "Latin Modern Roman", Georgia, serif;
  font-size: 16px;
  line-height: 1.5;
}

.pub-authors {
  color: #555;
}

.pub-authors strong {
  color: #1a1a1a;
}

.pub-venue {
  font-style: italic;
  color: #555;
}

.pub-badge {
  display: inline-block;
  margin-left: 8px;
  padding: 0 8px;
  border-radius: 999px;
  background-color: #fef3c7;
  color: #8a5300;
  font-family: Calibri, Carlito, "Segoe UI", sans-serif;
  font-size: 13px;
  font-style: normal;
  font-weight: bold;
  line-height: 1.7;
  vertical-align: 2px;
}

.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 10px;
}

.pub-link {
  display: inline-block;
  padding: 2px 13px;
  border: 1px solid var(--accent-border);
  border-radius: 999px;
  background-color: var(--accent-soft);
  color: var(--accent-dark) !important;
  font-size: 14px;
  font-weight: bold;
  line-height: 1.5;
  transition: background-color 0.15s, color 0.15s, border-color 0.15s;
}

.pub-link:hover {
  background-color: var(--accent);
  border-color: var(--accent);
  color: #fff !important;
  text-decoration: none;
}

.pub-legend {
  white-space: nowrap;
}

/* Tagline under the name */
.tagline {
  margin: 0 0 10px;
  font-size: 19px;
  font-weight: bold;
  color: var(--accent-dark);
}

/* Research-theme groups in the publication list */
.pub-group {
  margin-top: 30px;
}

.group-title {
  font-size: 22px !important;
  font-weight: bold !important;
  text-align: left !important;
  color: var(--text);
  margin: 0 0 2px !important;
}

.group-desc {
  margin: 0 0 4px;
  font-size: 16px;
  color: var(--muted);
}

/* One-line takeaway under each paper */
.pub-tldr {
  margin-top: 6px;
  font-size: 16px;
  line-height: 1.5;
  color: #333;
}

.show-earlier-btn {
  display: none;
}

/* Phones: compact header so the job banner fits in the first screen; cards stack; earlier work collapses */
@media (max-width: 760px) {
  .container {
    padding-left: 16px !important;
    padding-right: 16px !important;
  }
  .masthead {
    display: grid !important;
    grid-template-columns: 96px minmax(0, 1fr);
    column-gap: 16px;
    align-items: center !important;
    padding-top: 20px !important;
  }
  .site-info,
  .avatar-col {
    display: contents;
  }
  .social-icons {
    grid-column: 1 / -1;
    grid-row: 3;
    justify-content: flex-start;
    margin: 4px 0 0 -9px !important;
  }
  .site-avatar,
  .site-avatar img {
    width: 96px !important;
    height: 96px !important;
    border-radius: 10px !important;
  }
  .site-avatar {
    flex: none;
    margin: 0 !important;
    grid-column: 1;
    grid-row: 1;
  }
  .site-name {
    grid-column: 2;
    grid-row: 1;
    font-size: 30px !important;
    line-height: 1.15;
  }
  .about-section {
    grid-column: 1 / -1;
    grid-row: 2;
    margin-top: 14px;
    font-size: 17px;
    line-height: 1.6;
  }
  .tagline {
    font-size: 17px;
  }
  .bio-extra {
    display: none;
  }
  .job-market {
    padding: 16px 18px;
    font-size: 17px;
  }
  .job-market-title {
    font-size: 20px;
  }
  .job-market a.jm-btn {
    padding: 10px 18px;
  }
  .section-title {
    margin-top: 32px !important;
  }
  .group-title {
    font-size: 20px !important;
  }
  .paper {
    flex-direction: column;
    gap: 10px;
    padding: 14px;
  }
  .pub-thumb {
    flex-basis: auto;
    width: 100%;
    height: 150px;
  }
  .pub-title {
    font-size: 19px;
  }
  .pub-badge {
    margin-left: 0;
  }
  .pub-link {
    padding: 9px 16px;
    font-size: 15px;
  }
  .pub-links {
    gap: 10px;
  }
  .js .pub-group-earlier:not(.open) {
    display: none;
  }
  .js .show-earlier-btn {
    display: block;
    width: 100%;
    margin-top: 24px;
    padding: 12px;
    border: 1px solid var(--accent-border);
    border-radius: 999px;
    background-color: var(--accent-soft);
    color: var(--accent-dark);
    font: inherit;
    font-weight: bold;
    cursor: pointer;
  }
  .show-earlier-btn[hidden] {
    display: none !important;
  }
}
</style>


<div class="job-market">
<div class="job-market-text">
<div class="job-market-title">I'm on the job market!</div>
I'm looking for model training positions in San Francisco.
</div>
<div class="job-market-cta">
<a class="jm-btn" href="mailto:benjtherien@gmail.com">Email me</a>
<a class="jm-btn ghost" href="assets/Benjamin_Therien_CV.pdf">CV (PDF, updated Nov 2026)</a>
</div>
</div>

<h2 class="section-title">Selected Publications</h2>
<p class="section-sub">See my <a href="https://scholar.google.com/citations?hl=en&amp;user=RbO_ULYAAAAJ">Google Scholar</a> page for a complete list of publications, or download my <a href="assets/Benjamin_Therien_CV.pdf">CV</a>. <span class="pub-legend">* Equal contribution.</span></p>

<div class="pub-group" markdown="1">
<h3 class="group-title" id="distributed">Distributed &amp; communication-efficient pre-training</h3>
<p class="group-desc">Training LLMs across many workers and data centres with far less communication.</p>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/replica_scaling.webp" alt="Figure from How Inner Optimizers Shape Replica Scaling" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">How Inner Optimizers Shape Replica Scaling</div>
  <div class="pub-authors" markdown="span">Eugene Belilovsky, Stefan Horoi, Edouard Oyallon, **Benjamin Thérien**</div>
  <div class="pub-venue" markdown="span">Preprint</div>
  <div class="pub-tldr">Identifies pseudo-gradient covariance and batch-size noise as what drives DiLoCo's loss as replicas grow, and shows whitening-based inner optimizers scale well from 8 to 96 replicas.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2610.19064">ArXiv</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/2112261120509538386?s=20">Tweet Thread</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/model_merging.webp" alt="Figure from Can Model Merging Improve Aggregation in DiLoCo?" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Can Model Merging Improve Aggregation in DiLoCo?</div>
  <div class="pub-authors" markdown="span">Stefan Horoi, **Benjamin Thérien**, Guy Wolf, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">Advances in Neural Information Processing Systems (**NeurIPS**), 2026</div>
  <div class="pub-tldr">Treats DiLoCo's aggregation step as model merging and introduces IsoLoCo, which outperforms DiLoCo by a margin that widens as the number of workers grows.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2607.03011">ArXiv</a>
    <a class="pub-link" href="https://github.com/shoroi/isoloco">Code</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/covenant.webp" alt="Figure from Covenant-72B: Pre-Training a 72B LLM with Trustless Peers Over-the-Internet" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Covenant-72B: Pre-Training a 72B LLM with Trustless Peers Over-the-Internet</div>
  <div class="pub-authors" markdown="span">Joel Lidin, Amir Sarfi, Erfan Miahi, Quentin Anthony, Shivam Chauhan, Evangelos Pappas, **Benjamin Thérien**, Eugene Belilovsky, Samuel Dare</div>
  <div class="pub-venue" markdown="span">Preprint</div>
  <div class="pub-tldr">A 72B LLM pre-trained on about 1.1T tokens by open, permissionless peers using SparseLoCo: the largest collaborative globally distributed pre-training run, and competitive with centralized models.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2603.08163">ArXiv</a>
    <a class="pub-link" href="https://x.com/tplr_ai/status/2031388295972929720?s=20">Tweet Thread</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/muloco.webp" alt="Figure from MuLoCo: Muon is a Practical Inner Optimizer for DiLoCo" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">MuLoCo: Muon is a Practical Inner Optimizer for DiLoCo</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Xiaolong Huang, Aaron Defazio, Irina Rish, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">International Conference on Machine Learning (**ICML**), 2026</div>
  <div class="pub-tldr">Muon as DiLoCo's inner optimizer beats AdamW-based DiLoCo at every scale from 150M to 3.1B parameters; at 15B, 16-worker MuLoCo nearly matches single-worker training.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2505.23725">ArXiv</a>
    <a class="pub-link" href="https://bentherien.github.io/muloco-1/">Project Page</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/2026862326184304734?s=20">Tweet Thread</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/sparseloco.webp" alt="Figure from Communication Efficient LLM Pre-training with SparseLoCo" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Communication Efficient LLM Pre-training with SparseLoCo</div>
  <div class="pub-authors" markdown="span">Amir Sarfi, **Benjamin Thérien**, Joel Lidin, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">In Submission to International Conference on Machine Learning (**ICML**) 2026</div>
  <div class="pub-tldr">Top-k sparsification plus 2-bit quantization compresses pseudo-gradients by 97–99% while reaching lower loss than dense DiLoCo.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2508.15706">ArXiv</a>
    <a class="pub-link" href="https://x.com/amir_sarfi/status/1958714182750077215?s=20">Tweet Thread</a>
  </div>
</div>
</div>
</div>

<div class="pub-group" markdown="1">
<h3 class="group-title" id="learned-optimizers">Learned optimizers</h3>
<p class="group-desc">Meta-learned optimizers that generalize to larger models and are practical to use.</p>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/pylo.webp" alt="Figure from PyLO: Towards Accessible Learned Optimizers in PyTorch" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">PyLO: Towards Accessible Learned Optimizers in PyTorch</div>
  <div class="pub-authors" markdown="span">Paul Janson<sup title="Equal contribution">*</sup>, **Benjamin Thérien<sup title="Equal contribution">*</sup>**, Quentin Anthony, Xiaolong Huang, Abhinav Moudgil, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">Machine Learning and Systems (**MLSys**), 2026</div>
  <div class="pub-tldr">Brings learned optimizers such as VeLO to PyTorch through torch.optim, with CUDA kernels that raise ViT-B/16 training throughput roughly 4–5×.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2506.10315">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=Anr8OmuNK5">OpenReview</a>
    <a class="pub-link" href="https://github.com/Belilovsky-Lab/pylo">Code</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1934377825726865617?s=20">Tweet Thread</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/mulo.webp" alt="Figure from μLO: Compute-Efficient Meta-Generalization of Learned Optimizers" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">μLO: Compute-Efficient Meta-Generalization of Learned Optimizers</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Charles-Étienne Joseph, Boris Knyazev, Edouard Oyallon, Irina Rish, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">NeurIPS 2024 Workshop on Optimization for Machine Learning <span class="pub-badge">Oral</span></div>
  <div class="pub-venue" markdown="span">International Conference on Learning Representations (**ICLR**), 2026</div>
  <div class="pub-tldr">Deriving μP for learned optimizers improves meta-generalization to wider and deeper networks and to training horizons 25× longer than seen in meta-training, at the same compute.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2406.00153">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=LK9SPXbA05">OpenReview</a>
    <a class="pub-link" href="https://github.com/bentherien/mu_learned_optimization">Code</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1865930463098847575?s=20">Tweet Thread</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/local_l2o.webp" alt="Figure from Meta-learning Optimizers for Communication-Efficient Learning" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Meta-learning Optimizers for Communication-Efficient Learning</div>
  <div class="pub-authors" markdown="span">Charles-Étienne Joseph<sup title="Equal contribution">*</sup>, **Benjamin Thérien<sup title="Equal contribution">*</sup>**, Abhinav Moudgil, Boris Knyazev, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">Transactions on Machine Learning Research (**TMLR**), 2024</div>
  <div class="pub-tldr">Meta-learns the global update of local SGD, beating local-SGD variants while staying communication-efficient and generalizing to ImageNet, ViTs and language modeling.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2312.02204">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=uRbf9ANAns">OpenReview</a>
    <a class="pub-link" href="https://github.com/lefameuxbeding/learned_aggregation">Code</a>
  </div>
</div>
</div>
</div>

<div class="pub-group" markdown="1">
<h3 class="group-title" id="continual">Continual pre-training &amp; mixture-of-experts</h3>
<p class="group-desc">Updating LLMs with new data without re-training from scratch, and training better MoEs.</p>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/densebackprop.webp" alt="Figure from Dense Backpropagation Improves Routing for Sparsely-Gated Mixture-of-Experts" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Dense Backpropagation Improves Routing for Sparsely-Gated Mixture-of-Experts</div>
  <div class="pub-authors" markdown="span">Ashwinee Panda, Vatsal Baherwani, Zain Sarwar, **Benjamin Thérien**, Stephen Rawls, Sambit Sahu, Tom Goldstein, Supriyo Chakraborty</div>
  <div class="pub-venue" markdown="span">Advances in Neural Information Processing Systems (**NeurIPS**), 2025</div>
  <div class="pub-tldr">Gives the MoE router a dense gradient by filling in missing expert outputs with running averages, outperforming TopK routing with little overhead.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2504.12463">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=jTUIo4Kl6u">OpenReview</a>
    <a class="pub-link" href="https://anonymous.4open.science/r/default-moe-6C74/README.md">Code</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/cptofmoe.webp" alt="Figure from Continual Pre-training of MoEs: How robust is your router?" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Continual Pre-training of MoEs: How robust is your router?</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Charles-Étienne Joseph, Zain Sarwar, Ashwinee Panda, Anirban Das, Shi-Xiong Zhang, Stephen Rawls, Sambit Sahu, Eugene Belilovsky, Irina Rish</div>
  <div class="pub-venue" markdown="span">Transactions on Machine Learning Research (**TMLR**), 2025</div>
  <div class="pub-tldr">Across 600B-token runs, MoE routers stay robust to distribution shift during continual pre-training and match full re-training at a fraction of the cost.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2503.05029">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=dR7C1K71Rs">OpenReview</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1899909751049277668?s=20">Tweet Thread</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/sss.webp" alt="Figure from Simple and Scalable Strategies to Continually Pre-train Large Language Models" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Simple and Scalable Strategies to Continually Pre-train Large Language Models</div>
  <div class="pub-authors" markdown="span">Adam Ibrahim<sup title="Equal contribution">*</sup>, **Benjamin Thérien<sup title="Equal contribution">*</sup>**, Kshitij Gupta<sup title="Equal contribution">*</sup>, Mats Leon Richter, Quentin Anthony, Timothée Lesort, Eugene Belilovsky, Irina Rish</div>
  <div class="pub-venue" markdown="span">Transactions on Machine Learning Research (**TMLR**), 2024</div>
  <div class="pub-tldr">LR re-warming, re-decaying and replay match fully re-training LLMs up to 10B parameters, using a fraction of the compute.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2403.08763">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=DimPeeCxKO">OpenReview</a>
    <a class="pub-link" href="https://github.com/EleutherAI/gpt-neox/pull/1200">Code</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1768275963190640786?s=20">Tweet Thread</a>
    <a class="pub-link" href="https://youtu.be/y4sUn3sYWFc">Video</a>
  </div>
</div>
</div>
</div>

<button type="button" class="show-earlier-btn" aria-expanded="false" aria-controls="earlier-group">Show 3 earlier papers (2022–2024)</button>

<div class="pub-group pub-group-earlier" id="earlier-group" markdown="1">
<h3 class="group-title" id="earlier">Earlier work</h3>
<p class="group-desc">3D computer vision and signal processing.</p>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/rtmm.webp" alt="Figure from Object Re-Identification from Point Clouds" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Object Re-Identification from Point Clouds</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Chengjie Huang, Adrian Chow, Krzysztof Czarnecki</div>
  <div class="pub-venue" markdown="span">IEEE/CVF Winter Conference on Applications of Computer Vision (**WACV**), 2024</div>
  <div class="pub-tldr">The first large-scale study of object re-identification from LiDAR point clouds, reaching over 90% accuracy on rigid objects in real time.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://openaccess.thecvf.com/content/WACV2024/html/Therien_Object_Re-Identification_From_Point_Clouds_WACV_2024_paper.html">WACV</a>
    <a class="pub-link" href="https://arxiv.org/abs/2305.10210">ArXiv</a>
    <a class="pub-link" href="https://github.com/bentherien/point-cloud-reid">Code</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/itsc_im.webp" alt="Figure from Out-of-Distribution Detection for LiDAR-based 3D Object Detection" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Out-of-Distribution Detection for LiDAR-based 3D Object Detection</div>
  <div class="pub-authors" markdown="span">Chengjie Huang, Van Duong Nguyen, Vahdat Abdelzad, Christopher Mannes, Luke Rowe, **Benjamin Thérien**, Rick Salay, Krzysztof Czarnecki</div>
  <div class="pub-venue" markdown="span">IEEE 25th International Conference on Intelligent Transportation Systems (**ITSC**), 2022</div>
  <div class="pub-tldr">Adapts OOD detection methods to LiDAR 3D object detection and shows on KITTI that each method is biased toward particular OOD objects.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2209.14435">ArXiv</a>
  </div>
</div>
</div>

<div class="paper" markdown="1">
<div class="pub-thumb"><img src="{{ site.baseurl }}/images/thumbs/psn_im.webp" alt="Figure from Parametric Scattering Networks" loading="lazy" decoding="async"></div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Parametric Scattering Networks</div>
  <div class="pub-authors" markdown="span">Shanel Gauthier<sup title="Equal contribution">*</sup>, **Benjamin Thérien<sup title="Equal contribution">*</sup>**, Laurent Alsène-Racicot, Muawiz Chaudhary, Irina Rish, Eugene Belilovsky, Michael Eickenberg, Guy Wolf</div>
  <div class="pub-venue" markdown="span">IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR**), 2022 <span class="pub-badge">Oral · 4.2% of submissions</span></div>
  <div class="pub-tldr">Learning the scales, orientations and aspect ratios of Morlet wavelet filters gives significant gains over the standard scattering transform when labels are scarce.</div>
  <div class="pub-links">
    <a class="pub-link" href="https://openaccess.thecvf.com/content/CVPR2022/html/Gauthier_Parametric_Scattering_Networks_CVPR_2022_paper.html">CVPR</a>
    <a class="pub-link" href="https://arxiv.org/abs/2107.09539">ArXiv</a>
    <a class="pub-link" href="https://github.com/bentherien/parametricScatteringNetworks">Code</a>
    <a class="pub-link" href="https://www.youtube.com/watch?v=-B0ErCjQ9Nk">Video</a>
  </div>
</div>
</div>
</div>

<!-- - <div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/cpt_im.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>

**Continual Pre-Training of Large Language Models: How to re-warm your model?**<br/>
Kshitij Gupta*, **Benjamin Thérien***, Adam Ibrahim*, Mats Leon Richter, Quentin Anthony, Eugene Belilovsky, Timothée Lesort, Irina Rish<br/>
Efficient Systems for Foundation Models Workshop at **ICML** 2023<br/>
[ArXiv](https://arxiv.org/abs/2308.04014)
<div style="clear: both;"></div>
</div>-->

<!-- <div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/measeval_im.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>

- **CLaC-BP at SemEval-2021 Task 8 : SciBERT Plus Rules for MeasEval**<br/>
**Benjamin Therien**, Parsa Bagherzadeh, Sabine Bergler<br/>
Fifteenth Workshop on Semantic Evaluation (**SemEval**), 2021<br/>
[acl](https://aclanthology.org/2021.semeval-1.49/)

<div style="clear: both;"></div>
</div> -->

<script>
  /* Phones: "Earlier work" starts collapsed behind a button. Without JS everything stays visible. */
  (function () {
    document.documentElement.classList.add("js");
    var btn = document.querySelector(".show-earlier-btn");
    var group = document.getElementById("earlier-group");
    if (!btn || !group) return;
    btn.addEventListener("click", function () {
      group.classList.add("open");
      btn.setAttribute("aria-expanded", "true");
      btn.hidden = true;
    });
  })();
</script>
