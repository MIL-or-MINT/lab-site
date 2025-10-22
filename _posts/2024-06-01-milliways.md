---
layout: paper
category: paper
title: "Milliways: Taming Multiverses through Principled Evaluation of Data Analysis Paths"
authors: "Abhraneel Sarma, Kyle Hwang, Jessica Hullman, Matthew Kay"
venue: "ACM Human Factors in Computing Systems (CHI) 2024"
thumb: "assets/images/paper-thumb-milliways.png"
banner: "assets/images/paper-banner-milliways.jpg"
caption: "The Milliways interface consists of four panels to support the multiverse analysis tasks and a principled evaluation of the multiverse analysis. The outcome panel (A1) presents the results of the multiverse—for each universe in the multiverse, we show the outcome. The specification panel (A2) reveals the options for each parameter which the universe is composed of. The code panel (A3) presents the code that was used to construct the multiverse (here, the code was from the multiverse R library). The data panel (A4) shows the dataset used in the analysis. Other elements include the add button to add additional outcome variables (A5) , exclude button to remove options of a parameter (A6) , link button to link (aggregate) the outcomes across two or more options (A7) , slider for hierarchical sorting based on average effect (A8) and the zoom toggle (A9)."
pdf: "assets/papers/2024-milliways.pdf"
---

<!-- abstract -->

Multiverse analyses involve conducting all combinations of reasonable choices in a data analysis process. A reader of a study containing a multiverse analysis might question&mdash;are all the choices included in the multiverse reasonable and equally justifiable? How much do results vary if we make different choices in the analysis process? In this work, we identify principles for validating the composition of, and interpreting the uncertainty in, the results of a multiverse analysis. We present Milliways, a novel interactive visualisation system to support principled evaluation of multiverse analyses. Milliways provides interlinked panels presenting result distributions, individual analysis composition, multiverse code specification, and data summaries. Milliways supports interactions to sort, filter and aggregate results based on the analysis specification to identify decisions in the analysis process to which the results are sensitive. To represent the two qualitatively different types of uncertainty that arise in multiverse analyses—probabilistic uncertainty from estimating unknown quantities of interest such as regression coefficients, and possibilistic uncertainty from choices in the data analysis—Milliways uses consonance curves and probability boxes. Through an evaluative study with five users familiar with multiverse analysis, we demonstrate how Milliways can support multiverse analysis tasks, including a principled assessment of the results of a multiverse analysis.

<h3><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-bookmark" viewBox="0 0 16 16">
  <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"/>
</svg> Citation</h3>
<div class="bibtex">
<!-- bibtex -->
<h4>BibTeX</h4>
<pre>
@inproceedings{sarma2024milliways,
  title={Milliways: Taming multiverses through principled evaluation of data analysis paths},
  author={Sarma, Abhraneel and Hwang, Kyle and Hullman, Jessica and Kay, Matthew},
  booktitle={Proceedings of the 2024 CHI conference on human factors in computing systems},
  pages={1--15},
  year={2024}
}
</pre>
</div>
