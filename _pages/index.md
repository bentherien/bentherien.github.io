---
layout: page
title: 
permalink: /
---

<style>
/* Computer Modern (LaTeX) everywhere on the homepage */
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

body,
.site-name,
.site-description,
.page,
.page h1, .page h2, .page h3 {
  font-family: "CMU Serif", "Latin Modern Roman", Georgia, serif !important;
}

.page {
  font-size: 18px; /* Computer Modern runs small, so a bit larger than before */
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

/* Keep each paper's text beside its image, even when the text is taller */
.entry ul {
  overflow: hidden;
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

.paper ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.paper li strong:first-child {
  font-size: 21px;
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
- **How Inner Optimizers Shape Replica Scaling**<br/>
Eugene Belilovsky, Stefan Horoi, Edouard Oyallon, **Benjamin Thérien**<br/>
Preprint<br/>
[ArXiv](https://arxiv.org/abs/2610.19064) | [Tweet Thread](https://x.com/benjamintherien/status/2112261120509538386?s=20)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/covenant.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **Covenant-72B: Pre-Training a 72B LLM with Trustless Peers Over-the-Internet**<br/>
Joel Lidin, Amir Sarfi, Erfan Miahi, Quentin Anthony, Shivam Chauhan, Evangelos Pappas, **Benjamin Thérien**, Eugene Belilovsky, Samuel Dare<br/>
Preprint<br/>
[ArXiv](https://arxiv.org/pdf/2603.08163) | [Tweet Thread](https://x.com/tplr_ai/status/2031388295972929720?s=20)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/muloco.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **MuLoCo: Muon is a Practical Inner Optimizer for DiLoCo**<br/>
**Benjamin Thérien**, Xiaolong Huang, Aaron Defazio, Irina Rish, Eugene Belilovsky<br/>
In Submission to International Conference on Machine Learning (**ICML**) 2026<br/>
[ArXiv](https://arxiv.org/pdf/2505.23725) | [Project Page](https://bentherien.github.io/muloco-1/) | [Tweet Thread](https://x.com/benjamintherien/status/2026862326184304734?s=20)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/sparseloco.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **Communication Efficient LLM Pre-training with SparseLoCo**<br/>
Amir Sarfi, **Benjamin Thérien**, Joel Lidin, Eugene Belilovsky<br/>
In Submission to International Conference on Machine Learning (**ICML**) 2026<br/>
[ArXiv](https://arxiv.org/abs/2508.15706) | [Tweet Thread](https://x.com/amir_sarfi/status/1958714182750077215?s=20)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/pylo.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **PyLO: Towards Accessible Learned Optimizers in PyTorch**<br/>
Paul Janson`*`, **Benjamin Thérien`*`**, Quentin Anthony, Xiaolong Huang, Abhinav Moudgil, Eugene Belilovsky<br/>
Machine Learning and Systems (**MLSys**), 2026<br/>
[ArXiv](https://arxiv.org/pdf/2506.10315) | [OpenReview](https://openreview.net/forum?id=Anr8OmuNK5) | [Code](https://github.com/Belilovsky-Lab/pylo) | [Tweet Thread](https://x.com/benjamintherien/status/1934377825726865617?s=20)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/mulo.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **μLO: Compute-Efficient Meta-Generalization of Learned Optimizers**<br/>
**Benjamin Thérien**, Charles-Étienne Joseph, Boris Knyazev, Edouard Oyallon, Irina Rish, Eugene Belilovsky<br/>
(Oral) NeurIPS 2024 Workshop on Optimization for Machine Learning<br/>
International Conference on Learning Representations (**ICLR**), 2026<br/>
[ArXiv](https://arxiv.org/abs/2406.00153) | [OpenReview](https://openreview.net/forum?id=LK9SPXbA05) | [Code](https://github.com/bentherien/mu_learned_optimization) | [Tweet Thread](https://x.com/benjamintherien/status/1865930463098847575?s=20)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/densebackprop.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **Dense Backpropagation Improves Routing for Sparsely-Gated Mixture-of-Experts**<br/>
Ashwinee Panda, Vatsal Baherwani, Zain Sarwar, **Benjamin Thérien**, Stephen Rawls, Sambit Sahu, Tom Goldstein, Supriyo Chakraborty<br/>
Advances in Neural Information Processing Systems (**NeurIPS**), 2025<br/>
[ArXiv](https://arxiv.org/abs/2504.12463) | [OpenReview](https://openreview.net/forum?id=jTUIo4Kl6u) | [Code](https://anonymous.4open.science/r/default-moe-6C74/README.md)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/cptofmoe.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>
- **Continual Pre-training of MoEs: How robust is your router?**<br/>
**Benjamin Thérien**, Charles-Étienne Joseph, Zain Sarwar, Ashwinee Panda, Anirban Das, Shi-Xiong Zhang, Stephen Rawls, Sambit Sahu, Eugene Belilovsky, Irina Rish<br/>
Transactions on Machine Learning Research (**TMLR**), 2025<br/>
[ArXiv](https://arxiv.org/abs/2503.05029) | [OpenReview](https://openreview.net/forum?id=dR7C1K71Rs) | [Tweet Thread](https://x.com/benjamintherien/status/1899909751049277668?s=20)




<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/sss.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>

- **Simple and Scalable Strategies to Continually Pre-train Large Language Models**<br/>
Adam Ibrahim`*`, **Benjamin Thérien`*`**, Kshitij Gupta`*`, Mats Leon Richter, Quentin Anthony, Timothée Lesort, Eugene Belilovsky, Irina Rish<br/>
Transactions on Machine Learning Research (**TMLR**), 2024<br/>
[ArXiv](https://arxiv.org/pdf/2403.08763) | [OpenReview](https://openreview.net/forum?id=DimPeeCxKO) | [Code](https://github.com/EleutherAI/gpt-neox/pull/1200) | [Tweet Thread](https://x.com/benjamintherien/status/1768275963190640786?s=20) | [Video](https://youtu.be/y4sUn3sYWFc)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/local_l2o.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>

- **Meta-learning Optimizers for Communication-Efficient Learning**<br/>
Charles-Étienne Joseph`*`, **Benjamin Thérien**`*`, Abhinav Moudgil, Boris Knyazev, Eugene Belilovsky<br/>
Transactions on Machine Learning Research (**TMLR**), 2024<br/>
[ArXiv](https://arxiv.org/abs/2312.02204) | [OpenReview](https://openreview.net/forum?id=uRbf9ANAns) | [Code](https://github.com/lefameuxbeding/learned_aggregation)

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

- **Object Re-Identification from Point Clouds**<br/>
**Benjamin Thérien**, Chengjie Huang, Adrian Chow, Krzysztof Czarnecki<br/>
IEEE/CVF Winter Conference on Applications of Computer Vision (**WACV**), 2024<br/>
[WACV](https://openaccess.thecvf.com/content/WACV2024/html/Therien_Object_Re-Identification_From_Point_Clouds_WACV_2024_paper.html) | [ArXiv](https://arxiv.org/abs/2305.10210) | [Code](https://github.com/bentherien/point-cloud-reid)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/itsc_im.png" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>


- **Out-of-Distribution Detection for LiDAR-based 3D Object Detection**<br/>
Chengjie Huang, Van Duong Nguyen, Vahdat Abdelzad, Christopher Mannes, Luke Rowe, **Benjamin Thérien**, Rick Salay, Krzysztof Czarnecki<br/>
IEEE 25th International Conference on Intelligent Transportation Systems (**ITSC**), 2022<br/>
[ArXiv](https://arxiv.org/abs/2209.14435)

<div style="clear: both;"></div>
</div>

<div class="paper" markdown="1">
<div style="width: 25%; float: left; margin: 5px 25px 5px 5px; text-align: right;">
  <img src="{{ site.baseurl }}/images/psn_im.gif" style="max-height: 150px; border: 1px solid #ddd; padding: 5px; background-color: #f9f9f9;">
</div>

- **(oral: 4.2% of submissions) Parametric Scattering Networks**<br/>
Shanel Gauthier`*`, **Benjamin Thérien`*`†**], Laurent Alsène-Racicot, Muawiz Chaudhary, Irina Rish, Eugene Belilovsky, Michael Eickenberg, Guy Wolf<br/>
IEEE/CVF Conference on Computer Vision and Pattern Recognition (**CVPR**), 2022<br/>
[CVPR](https://openaccess.thecvf.com/content/CVPR2022/html/Gauthier_Parametric_Scattering_Networks_CVPR_2022_paper.html) | [ArXiv](https://arxiv.org/abs/2107.09539) | [Code](https://github.com/bentherien/parametricScatteringNetworks) | [Video](https://www.youtube.com/watch?v=-B0ErCjQ9Nk)

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
