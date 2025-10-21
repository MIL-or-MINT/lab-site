---
layout: paper
category: paper
title: "A Decision Theoretic Framework for Measuring AI Reliance"
authors: "Ziyang Guo, Yifan Wu, Jason Hartline, Jessica Hullman"
venue: "ACM Conference on Fairness, Accountability, and Transparency (ACM FAccT '24)"
thumb: "assets/images/paper-thumb-dt-framework.png"
banner: "assets/images/paper-banner-dt-framework.png"
caption: "Expected payoffs of benchmarks, baselines, and observed performance in Bansal et al. in which the performance of human-AI teams (behavioral decision score, orange) overperforms human alone (human alone score, pink) or AI alone (rational baseline, green). The behavioral loss sourced from over-/under-reliance of human-AI teams (determined by the distance between mis-reliant benchmark and rational benchmark) only takes a small proportion compared with other sources."
pdf: "assets/papers/2024-dt-framework.pdf"
---

<!-- abstract -->

Humans frequently make decisions with the aid of artificially intelligent (AI) systems. A common pattern is for the AI to recommend an action to the human who retains control over the final decision. Researchers have identified ensuring that a human has appropriate reliance on an AI as a critical component of achieving complementary performance. We argue that the current definition of appropriate reliance used in such research lacks formal statistical grounding and can lead to contradictions. We propose a formal definition of reliance, based on statistical decision theory, which separates the concepts of reliance as the probability the decision-maker follows the AI’s recommendation from challenges a human may face in differentiating the signals and forming accurate beliefs about the situation. Our definition gives rise to a framework that can be used to guide the design and interpretation of studies on human-AI complementarity and reliance. Using recent AI-advised decision making studies from literature, we demonstrate how our framework can be used to separate the loss due to mis-reliance from the loss due to not accurately differentiating the signals. We evaluate these losses by comparing to a baseline and a benchmark for complementary performance defined by the expected payoff achieved by a rational decision-maker facing the same decision task as the behavioral decision-makers.

<h3><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-bookmark" viewBox="0 0 16 16">
  <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"/>
</svg> Citation</h3>
<div class="bibtex">
<!-- bibtex -->
<h4>BibTeX</h4>
<pre>
@inproceedings{guo2024decision,
  title={A decision theoretic framework for measuring AI reliance},
  author={Guo, Ziyang and Wu, Yifan and Hartline, Jason D and Hullman, Jessica},
  booktitle={Proceedings of the 2024 ACM Conference on Fairness, Accountability, and Transparency},
  pages={221--236},
  year={2024}
}
</pre>
</div>
