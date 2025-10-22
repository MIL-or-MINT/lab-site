---
layout: paper
category: paper
title: "Designing Shared Information Displays for Agents of Varying Strategic Sophistication"
authors: "Dongping Zhang, Jason Hartline, Jessica Hullman"
venue: "ACM Computer-Supported Cooperative Work (CSCW) 2024"
thumb: "assets/images/paper-thumb-strategic-display.gif"
banner: "assets/images/paper-banner-strategic-display.png"
caption: "Diagram of key features of our experimental design. (1) We define a pseudo-Poisson distribution using a <math><mi>Poisson</mi><mo>(</mo><mn>1.5</mn><mo>)</mo></math>, which includes <math><mi>L0</mi></math>s&mdash;<math><mi>L2</mi></math>s. (2) We endow level-specific beliefs by normalizing the pseudo-Poisson distribution for <math><mi>L1</mi></math>s and <math><mi>L2</mi></math>s who are our study participants. (3) We conduct a staged data collection: in each trial, participants use an information display to make decisions and then review a level-specific feedback. <math><mi>L1</mi></math>s and <math><mi>L2</mi></math>s complete all trials in the same order, but <math><mi>L1</mi></math>s complete the study before <math><mi>L2</mi></math>s, so that <math><mi>L1</mi></math>s' responses can be used with that of <math><mi>L0</mi></math>s (i.e., the taxi data) to construct a level-specific feedback that aligns with <math><mi>L2</mi></math>s' endowed belief. (4) We calculate the system outcome by combining decisions from <math><mi>L0</mi></math>s (i.e., the taxi data) and <math><mi>L1</mi></math>s&mdash;<math><mi>L2</mi></math>s (i.e., the collected responses) according to the mixture we used to define the level distribution (step 1). (5) We conduct two replications of the experiment by varying trial order and re-define the level mixture of <math><mi>L0</mi></math>s&mdash;<math><mi>L2</mi></math>s using a <math><mi>Poisson</mi><mo>(</mo><mn>3</mn><mo>)</mo></math>."
pdf: "assets/papers/2024-strategic-display.pdf"
supplementary: "https://github.com/dpzhang/shared-info-display"
---

<!-- abstract -->

Data-driven predictions are often perceived as inaccurate in hindsight due to behavioral responses. We consider the role of interface design choices on how individuals respond to predictions presented on a shared information display in a strategic setting. We introduce a novel staged experimental design to investigate the effects of interface design features, such as the visualization of prediction uncertainty and prediction error, within a repeated congestion game. In this game, participants assume the role of taxi drivers and use a shared information display to decide where to search for their next ride. Our experimental design endows agents with varying level-<i>k</i> depths of thinking, allowing some agents to possess greater sophistication in anticipating the decisions of others using the same information display. Through several large pre-registered experiments, we identify trade-offs between displays that are optimal for individual decisions and those that best serve the collective social welfare of the system. Additionally, we note that the influence of display characteristics varies based on an agent's strategic sophistication. We observe that design choices promoting individual-level decision-making can lead to suboptimal system outcomes, as manifested by a lower realization of potential social welfare. However, this decline in social welfare is offset by a slight reduction in distribution shift, narrowing the gap between predicted and realized system outcomes. This may enhance the perceived reliability and trustworthiness of the information display post hoc. Our findings pave the way for new research questions concerning the design of effective prediction interfaces in strategic environments.

<h3><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-bookmark" viewBox="0 0 16 16">
  <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"/>
</svg> Citation</h3>
<div class="bibtex">
<!-- bibtex -->
<h4>BibTeX</h4>
<pre>
@article{zhang2024designing,
  title={Designing Shared Information Displays for Agents of Varying Strategic Sophistication},
  author={Zhang, Dongping and Hartline, Jason and Hullman, Jessica},
  journal={Proceedings of the ACM on Human-Computer Interaction},
  volume={8},
  number={CSCW1},
  pages={1--34},
  year={2024},
  publisher={ACM New York, NY, USA}
  doi={https://doi.org/10.1145/3637319}
}
</pre>
</div>
