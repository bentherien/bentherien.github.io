---
layout: page
title: 
permalink: /
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Carlito:ital,wght@0,400;0,700;1,400;1,700&display=swap');

/* Computer Modern (LaTeX), used for author lists and venues */
@font-face {
  font-family: "CMU Serif";
  font-style: normal;
  font-weight: 400;
  src: url("/fonts/cmu/cmu-serif-500-roman.woff2") format("woff2");
}

@font-face {
  font-family: "CMU Serif";
  font-style: normal;
  font-weight: 700;
  src: url("/fonts/cmu/cmu-serif-700-roman.woff2") format("woff2");
}

@font-face {
  font-family: "CMU Serif";
  font-style: italic;
  font-weight: 400;
  src: url("/fonts/cmu/cmu-serif-500-italic.woff2") format("woff2");
}

@font-face {
  font-family: "CMU Serif";
  font-style: italic;
  font-weight: 700;
  src: url("/fonts/cmu/cmu-serif-700-italic.woff2") format("woff2");
}

/* Calibri, falling back to Carlito (a metric-compatible open clone) where Calibri isn't installed */
body,
.site-name,
.site-description,
.page,
.page h1, .page h2, .page h3 {
  font-family: Calibri, Carlito, "Segoe UI", sans-serif !important;
}

.page {
  font-size: 18px;
  line-height: 1.7;
}

.container {
  max-width: 1800px !important; /* Narrower content area = wider margins */
  padding-left: 60px !important; /* Additional padding on left */
  padding-right: 60px !important; /* Additional padding on right */
}

/* Profile/Avatar image size - Bigger! */
.site-avatar {
  width: 310px !important;
  height: 310px !important;
  float: left !important;
  margin-right: 40px !important;
  margin-top: 0 !important;
}

.site-avatar img {
  width: 310px !important;
  height: 310px !important;
}

/* Move name and affiliation to top */
.site-info {
  float: none !important;
  margin-top: 0 !important;
  text-align: left !important;
  margin-bottom: 20px !important;
}

.site-name {
  font-size: 36px !important;
  letter-spacing: normal !important;
  font-weight: bold !important;
  text-align: left !important;
  margin-bottom: 0 !important;
}

.site-description {
  font-size: 18px !important;
  margin-top: 0 !important;
  margin-bottom: 0 !important;
}

/* Custom header layout */
.custom-header {
  margin-bottom: 30px;
  overflow: auto;
}

/* About Me sits in the header, to the right of the photo */
.site-info {
  overflow: hidden !important;
}

/* On narrow screens, stack the photo above the bio */
@media (max-width: 760px) {
  .site-avatar {
    float: none !important;
    display: block;
    margin: 0 auto 20px auto !important;
  }
  .site-info {
    overflow: visible !important;
  }
  .paper > div:first-child {
    width: 100% !important;
    float: none !important;
    margin: 0 0 12px 0 !important;
    text-align: center !important;
  }
}

.about-section {
  margin-top: 20px;
  clear: none;
  font-size: 18px;
  line-height: 1.7;
}

.job-market {
  margin-top: 25px;
  padding: 20px 26px;
  border-radius: 10px;
  background: linear-gradient(135deg, #1f6fd1, #3b8cf0);
  color: #fff;
  font-size: 18px;
  line-height: 1.6;
  box-shadow: 0 4px 14px rgba(31, 111, 209, 0.3);
}

.job-market-title {
  font-size: 22px;
  font-weight: bold;
  margin-bottom: 4px;
}

.job-market a {
  color: #fff;
  font-weight: bold;
  text-decoration: underline;
}

/* Each paper is a card */
.paper {
  margin: 20px 0;
  padding: 16px 20px;
  border: 1px solid #e3e6ea;
  border-radius: 10px;
  background-color: #fff;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.06);
  transition: box-shadow 0.2s, border-color 0.2s;
}

.paper:hover {
  border-color: #b9d2f3;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.1);
}

.paper-body {
  overflow: hidden; /* keep the text beside the thumbnail */
}

.pub-title {
  font-size: 21px;
  font-weight: bold;
  line-height: 1.35;
  margin-bottom: 4px;
}

.pub-authors,
.pub-venue {
  font-family: "CMU Serif", "Latin Modern Roman", Georgia, serif;
  font-size: 17px;
  line-height: 1.5;
}

.pub-authors {
  color: #555;
}

.pub-authors strong {
  color: #222;
}

.pub-venue {
  font-style: italic;
  color: #555;
  margin-top: 2px;
}

.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 10px;
}

.pub-link {
  display: inline-block;
  padding: 0 10px;
  border: 1px solid #4183C4;
  border-radius: 4px;
  font-size: 14px;
  font-weight: bold;
  line-height: 1.7;
  color: #4183C4;
  transition: background-color 0.15s, color 0.15s;
}

.pub-link:hover {
  background-color: #4183C4;
  color: #fff !important;
  text-decoration: none;
}
</style>


<a href="https://github.com/bentherien">
<img src="assets/github.png" height="45" style="float:top; margin:5px"></a>
<a href="https://scholar.google.com/citations?hl=en&user=RbO_ULYAAAAJ">
<img src="assets/google_scholar.png" height="45" style="float:top; margin:5px"></a>
<a href="https://www.linkedin.com/in/benjamintherien/">
<img src="assets/linkedin.png" height="45" style="float:top; margin:5px"></a>
<a href="https://x.com/benjamintherien">
<img src="assets/x.png" height="45" style="float:top; margin:5px"></a>
<a href="mailto:benjtherien@gmail.com">
<img src="assets/gmail.png" height="45" style="float:top; margin:5px"></a>
<a href="assets/Benjamin_Therien_CV.pdf">
<img src="assets/cv.png" height="45" alt="CV" title="CV" style="float:top; margin:5px"></a>

<div class="job-market">
<div class="job-market-title">I'm on the job market!</div>
I'm looking for model training positions in San Francisco. Feel free to reach out by <a href="mailto:benjtherien@gmail.com">email</a>.
</div>

<div style="clear: both; padding-top: 20px;"></div>


<div style="text-align: left; font-size: 28px;">
Selected Publications
</div>
See my [Google Scholar](https://scholar.google.com/citations?hl=en&user=RbO_ULYAAAAJ) page for a complete list of publications, or download my [CV](assets/Benjamin_Therien_CV.pdf).



<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/replica_scaling.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">How Inner Optimizers Shape Replica Scaling</div>
  <div class="pub-authors" markdown="span">Eugene Belilovsky, Stefan Horoi, Edouard Oyallon, **Benjamin Thérien**</div>
  <div class="pub-venue" markdown="span">Preprint</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2610.19064">ArXiv</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/2112261120509538386?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/covenant.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Covenant-72B: Pre-Training a 72B LLM with Trustless Peers Over-the-Internet</div>
  <div class="pub-authors" markdown="span">Joel Lidin, Amir Sarfi, Erfan Miahi, Quentin Anthony, Shivam Chauhan, Evangelos Pappas, **Benjamin Thérien**, Eugene Belilovsky, Samuel Dare</div>
  <div class="pub-venue" markdown="span">Preprint</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2603.08163">ArXiv</a>
    <a class="pub-link" href="https://x.com/tplr_ai/status/2031388295972929720?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/muloco.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">MuLoCo: Muon is a Practical Inner Optimizer for DiLoCo</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Xiaolong Huang, Aaron Defazio, Irina Rish, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">In Submission to International Conference on Machine Learning (**ICML**) 2026</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2505.23725">ArXiv</a>
    <a class="pub-link" href="https://bentherien.github.io/muloco-1/">Project Page</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/2026862326184304734?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/sparseloco.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Communication Efficient LLM Pre-training with SparseLoCo</div>
  <div class="pub-authors" markdown="span">Amir Sarfi, **Benjamin Thérien**, Joel Lidin, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">In Submission to International Conference on Machine Learning (**ICML**) 2026</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2508.15706">ArXiv</a>
    <a class="pub-link" href="https://x.com/amir_sarfi/status/1958714182750077215?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/pylo.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">PyLO: Towards Accessible Learned Optimizers in PyTorch</div>
  <div class="pub-authors" markdown="span">Paul Janson`*`, **Benjamin Thérien`*`**, Quentin Anthony, Xiaolong Huang, Abhinav Moudgil, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">Machine Learning and Systems (**MLSys**), 2026</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2506.10315">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=Anr8OmuNK5">OpenReview</a>
    <a class="pub-link" href="https://github.com/Belilovsky-Lab/pylo">Code</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1934377825726865617?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/mulo.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">μLO: Compute-Efficient Meta-Generalization of Learned Optimizers</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Charles-Étienne Joseph, Boris Knyazev, Edouard Oyallon, Irina Rish, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">(Oral) NeurIPS 2024 Workshop on Optimization for Machine Learning</div>
  <div class="pub-venue" markdown="span">International Conference on Learning Representations (**ICLR**), 2026</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2406.00153">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=LK9SPXbA05">OpenReview</a>
    <a class="pub-link" href="https://github.com/bentherien/mu_learned_optimization">Code</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1865930463098847575?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/densebackprop.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Dense Backpropagation Improves Routing for Sparsely-Gated Mixture-of-Experts</div>
  <div class="pub-authors" markdown="span">Ashwinee Panda, Vatsal Baherwani, Zain Sarwar, **Benjamin Thérien**, Stephen Rawls, Sambit Sahu, Tom Goldstein, Supriyo Chakraborty</div>
  <div class="pub-venue" markdown="span">Advances in Neural Information Processing Systems (**NeurIPS**), 2025</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2504.12463">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=jTUIo4Kl6u">OpenReview</a>
    <a class="pub-link" href="https://anonymous.4open.science/r/default-moe-6C74/README.md">Code</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/cptofmoe.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Continual Pre-training of MoEs: How robust is your router?</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Charles-Étienne Joseph, Zain Sarwar, Ashwinee Panda, Anirban Das, Shi-Xiong Zhang, Stephen Rawls, Sambit Sahu, Eugene Belilovsky, Irina Rish</div>
  <div class="pub-venue" markdown="span">Transactions on Machine Learning Research (**TMLR**), 2025</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2503.05029">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=dR7C1K71Rs">OpenReview</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1899909751049277668?s=20">Tweet Thread</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/sss.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Simple and Scalable Strategies to Continually Pre-train Large Language Models</div>
  <div class="pub-authors" markdown="span">Adam Ibrahim`*`, **Benjamin Thérien`*`**, Kshitij Gupta`*`, Mats Leon Richter, Quentin Anthony, Timothée Lesort, Eugene Belilovsky, Irina Rish</div>
  <div class="pub-venue" markdown="span">Transactions on Machine Learning Research (**TMLR**), 2024</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/pdf/2403.08763">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=DimPeeCxKO">OpenReview</a>
    <a class="pub-link" href="https://github.com/EleutherAI/gpt-neox/pull/1200">Code</a>
    <a class="pub-link" href="https://x.com/benjamintherien/status/1768275963190640786?s=20">Tweet Thread</a>
    <a class="pub-link" href="https://youtu.be/y4sUn3sYWFc">Video</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/local_l2o.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Meta-learning Optimizers for Communication-Efficient Learning</div>
  <div class="pub-authors" markdown="span">Charles-Étienne Joseph`*`, **Benjamin Thérien**`*`, Abhinav Moudgil, Boris Knyazev, Eugene Belilovsky</div>
  <div class="pub-venue" markdown="span">Transactions on Machine Learning Research (**TMLR**), 2024</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2312.02204">ArXiv</a>
    <a class="pub-link" href="https://openreview.net/forum?id=uRbf9ANAns">OpenReview</a>
    <a class="pub-link" href="https://github.com/lefameuxbeding/learned_aggregation">Code</a>
  </div>
</div>
<div style="clear: both;"></div>
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


<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/rtmm.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Object Re-Identification from Point Clouds</div>
  <div class="pub-authors" markdown="span">**Benjamin Thérien**, Chengjie Huang, Adrian Chow, Krzysztof Czarnecki</div>
  <div class="pub-venue" markdown="span">IEEE/CVF Winter Conference on Applications of Computer Vision (**WACV**), 2024</div>
  <div class="pub-links">
    <a class="pub-link" href="https://openaccess.thecvf.com/content/WACV2024/html/Therien_Object_Re-Identification_From_Point_Clouds_WACV_2024_paper.html">WACV</a>
    <a class="pub-link" href="https://arxiv.org/abs/2305.10210">ArXiv</a>
    <a class="pub-link" href="https://github.com/bentherien/point-cloud-reid">Code</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/itsc_im.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">Out-of-Distribution Detection for LiDAR-based 3D Object Detection</div>
  <div class="pub-authors" markdown="span">Chengjie Huang, Van Duong Nguyen, Vahdat Abdelzad, Christopher Mannes, Luke Rowe, **Benjamin Thérien**, Rick Salay, Krzysztof Czarnecki</div>
  <div class="pub-venue" markdown="span">IEEE 25th International Conference on Intelligent Transportation Systems (**ITSC**), 2022</div>
  <div class="pub-links">
    <a class="pub-link" href="https://arxiv.org/abs/2209.14435">ArXiv</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/psn_im.gif" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
<div class="paper-body" markdown="1">
  <div class="pub-title" markdown="span">(oral: 4.2% of submissions) Parametric Scattering Networks</div>
  <div class="pub-authors" markdown="span">Shanel Gauthier`*`, **Benjamin Thérien`*`†**, Laurent Alsène-Racicot, Muawiz Chaudhary, Irina Rish, Eugene Belilovsky, Michael Eickenberg, Guy Wolf</div>
  <div class="pub-venue" markdown="span">IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR**), 2022</div>
  <div class="pub-links">
    <a class="pub-link" href="https://openaccess.thecvf.com/content/CVPR2022/html/Gauthier_Parametric_Scattering_Networks_CVPR_2022_paper.html">CVPR</a>
    <a class="pub-link" href="https://arxiv.org/abs/2107.09539">ArXiv</a>
    <a class="pub-link" href="https://github.com/bentherien/parametricScatteringNetworks">Code</a>
    <a class="pub-link" href="https://www.youtube.com/watch?v=-B0ErCjQ9Nk">Video</a>
  </div>
</div>
<div style="clear: both;"></div>
</div>

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

---
<small>†: Oral presenter. *: Equal contribution.</small>
