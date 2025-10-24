---
layout: paper
category: paper
title: "Evaluating the Utility of Conformal Prediction Sets for AI-Advised Image Labeling"
authors: "Dongping Zhang, Angelos Chatzimparmpas, Negar Kamali, Jessica Hullman"
venue: "ACM Human Factors in Computing Systems (CHI) 2024"
thumb: "assets/images/paper-thumb-conformal-utility.png"
banner: "assets/images/paper-banner-conformal-utility.png"
caption: "Overview diagram of our key experimental manipulations: (1) Five different covariate shifts are imposed through synthetic image corruption to create five replications of the conformal hold-out set, each containing images that are out-of-distribution (OOD). (2) Images in each conformal hold-out set are categorized by the classifier's prediction confidence for difficulty and the size of the derived set. Ten task images representative of the categories used to define each group are selected. (3) Participants label 16 task images sampled from 80 candidate images: four in-distribution and 12 OOD, balanced by difficulty and set size, presented in randomized order. (4) Based on the conditions assigned, participants may complete labeling tasks without predictions (i.e., <span style='color:#4E79A7; font-weight:bold'>baseline</span>) or with access to prediction displays that vary in the content provided by uncertainty quantification (i.e., <span style='color:#F28E2B; font-weight:bold'>Top-1</span>, <span style='color:#E15759; font-weight:bold'>Top-10</span>, or <span style='color:#76B7B2; font-weight:bold'>prediction set</span>)."
pdf: "assets/papers/2024-conformal-utility.pdf"
github: "https://github.com/dpzhang/conformal-prediction-utility"
honorable: true
---

<!-- abstract -->

As deep neural networks are more commonly deployed in high-stakes domains, their black-box nature makes uncertainty quantification challenging. We investigate the effects of presenting conformal prediction sets&mdash;a distribution-free class of methods for generating prediction sets with specified coverage&mdash;to express uncertainty in AI-advised decision-making. Through a large online experiment, we compare the utility of conformal prediction sets to displays of Top-1 and Top-<i>k</i> predictions for AI-advised image labeling. In a pre-registered analysis, we find that the utility of prediction sets for accuracy varies with the difficulty of the task: while they result in accuracy on par with or less than Top-1 and Top-<i>k</i> displays for easy images, prediction sets excel at assisting humans in labeling out-of-distribution (OOD) images, especially when the set size is small. Our results empirically pinpoint practical challenges of conformal prediction sets and provide implications on how to incorporate them for real-world decision-making.

<h3><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-bookmark" viewBox="0 0 16 16">
  <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"/>
</svg> Citation</h3>
<div class="bibtex">
<!-- bibtex -->
<h4>BibTeX</h4>
<pre>
@inproceedings{zhang2024evaluating,
  title={Evaluating the utility of conformal prediction sets for ai-advised image labeling},
  author={Zhang, Dongping and Chatzimparmpas, Angelos and Kamali, Negar and Hullman, Jessica},
  booktitle={Proceedings of the 2024 CHI Conference on Human Factors in Computing Systems},
  pages={1--19},
  year={2024},
  doi={https://doi.org/10.1145/3613904.3642446}
}
</pre>
</div>
