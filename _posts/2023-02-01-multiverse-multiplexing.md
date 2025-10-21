---
layout: paper
category: paper
title: "multiverse: Multiplexing Alternative Data Analyses in R Notebooks"
authors: "Abhraneel Sarma, Alex Kale, Michael Moon, Nathan Taback, Fanny Chevalier, Jessica Hullman, Matthew Kay"
venue: "ACM Human Factors in Computing Systems (CHI) 2023"
thumb: "assets/images/paper-thumb-multiverse-multiplexing.png"
banner: "assets/images/paper-banner-multiverse-multiplexing.png"
caption: "User can define procedural dependencies between options with the %when% operator. Users can also reuse parameter names for decisions which manifest in more than one location."
pdf: "assets/papers/2023-multiverse-multiplexing.pdf"
honorable: true
---

<!-- abstract -->

There are myriad ways to analyze any given dataset. But which one to trust? In the face of such uncertainty, analysts adopt multiverse analysis: running all reasonable analyses on the dataset. Yet this is cognitively and technically difficult with existing tools—how does one specify and execute all combinations of reasonable analyses of a dataset?—and often requires discarding existing workflows. We present multiverse, a tool for implementing multiverse analyses in R with expressive syntax supporting existing computational notebook workflows. Informed by iterative user testing, multiverse supports building up a multiverse through local changes to a single analysis and optimises execution by pruning redundant computations. We evaluate four existing multiverse tools (including multiverse) using principles of cognitive ergonomics.We identify design tradeoffs (e.g. flexibility in locally defining decisions versus making it easy to understand a multiverse’s global structure), and suggest future directions for multiverse tool design, like more effective debugging support.

<h3><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-bookmark" viewBox="0 0 16 16">
  <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"/>
</svg> Citation</h3>
<div class="bibtex">
<!-- bibtex -->
<h4>BibTeX</h4>
<pre>
@inproceedings{sarma2023multiverse,
	title        = {multiverse: Multiplexing alternative data analyses in R notebooks},
	author       = {Sarma, Abhraneel and Kale, Alex and Moon, Michael Jongho and Taback, Nathan and Chevalier, Fanny and Hullman, Jessica and Kay, Matthew},
	booktitle    = {Proceedings of the 2023 CHI conference on human factors in computing systems},
	pages        = {1--15},
	year         = {2023}
}
</pre>
</div>
