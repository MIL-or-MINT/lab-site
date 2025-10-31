# Model Decisions (MODE) Lab Website

This repository hosts the in-progress site for Jessica Hullman's **Mo**del **De**cisions (MODE) Lab. Our lab site is built with `Jekyll` and this repo stores all supporting assets (e.g., images, paper PDFs, metadata, etc.).

> Note: If you are not a developer or the designated webmaster, you do not need to clone or modify this repository.

## :busts_in_silhouette: Staff

Hyeok Kim - rebuilding the template :man_technologist:

Lily Ge - building individual `.md` files :woman_technologist:

Fumeng Yang - writing documentation & refining style :woman_juggling:

Dongping Zhang - standing on the shoulders of these giants and put the final nail in the coffin :hammer:

## :calendar: Before You Start

Each academic year, one lab member will serve as the webmaster, responsible for maintaining and updating the site.
Other members should send update requests to the webmaster via the Slack channel #logo-and-website or by direct message.

> The 2025 webmaster is Dongping Zhang.

## :wrench: How to update

For site maintaince and content update, the webmaster will primarily work within three directories: `_data`, `_posts`, and `assets`.

After making edits, wait a few minutes and check the live site ([#TODO URL]) to verify that changes have propagated.

### 1. Updating the Publications Page :page_facing_up:

To update the `Publications` page, the webmaster should first collect these assets from the paper's lead author:

1. Thumbnail image
2. Banner/teaser **with caption, formatted for HTML**
3. Abstract with HTML formating
4. Final paper pdf.

Updates mainly involve two directories: `_posts` and `assets`.

Each new paper requires a **unique**, **concise**, and **professional** ID. Example ID: `awesome-paper`.

#### 1.1 Upload the Paper Assets to `assets/`

1. **Thumbnail**

   - Aspect ratio: 5 : 3
   - Recommended width ≤ 300 px (ideal ≈ 200 × 120 px)
   - Name format: `paper-thumb-awesome-paper.[png|jpg|jpeg|gif|bmp]`
   - Upload to: `assets/images/`

2. **Banner/Teaser**

   - Max width ≈ 1200 px (avoid small text, since it scales down on mobile ≈ 400 px)
   - Name format: `paper-banner-awesome-paper.[png|jpg|jpeg|gif|bmp]`
   - Upload to: `assets/images/`

3. **Paper PDF**
   - Name format: `yyyy-awesome-paper.pdf`
   - Upload to: `assets/papers/`

#### 1.2 Create/Modify Markdown in `_posts/`

Each `md` file serves as the entry to render unique paper page. To add a new paper, create a new `md` file in `_post` and **must** name it as: `yyyy-mm-dd-[awesome]-[paper].md`. The exact month and date are not important. Use ascending numerical values for easier ordering (e.g., 2025-01-01, 2025-02-01, etc.).

The example below shows the recommended structure of a paper entry. You can copy it as a template.

> Please review it carefully to ensure formatting and style remain consistent across pages.

```{yaml}
---
layout: paper
category: paper
title:  "Copy and paste the paper title"
authors: "Author 1, Author 2, Author 3 -- pay attention to the formatting: do not add an "and" before the last author"
venue: "The Lucky Conference/Journal"
thumb: "assets/images/paper-thumb-awesome-paper.png"
banner: "assets/images/paper-banner-awesome-paper.png"
caption: "The caption for the banner/teaser."
pdf: "assets/papers/yyyy-mm-dd-awesome-paper.pdf"
bestPaper: true
honorable: false
github: "github.com/awesome"
supplementary: "https://osf.io/awesome/"
additionals:
  - name: "Gallery"
    link: "https://awesomepaper.com"
  - name: "Package"
    link: "https://github.com"
  - name: "Documentation"
    link: "https://documentation.com"
  - name: "Online Editor"
    link: "https://editor.com"
---

<!-- abstract -->
[Put abstract here with html formatting and adjustment]

<h3><svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="bi bi-bookmark" viewBox="0 0 16 16">
  <path d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"/>
</svg> Citation</h3>
<div class="bibtex">
<!-- bibtex -->
<h4>Bibtex</h4>
<pre>
@article{paper-id-year,
  ...
}
</pre>
</div>
```

**Notes:**

- **author**: ensure consistent formatting and do not include “and” before the last author.
- **bestPaper** / **honorable**: falg it as `true` or `false`. If the paper received no award, you can omit these fields.
- **github** / **supplementary**: include links if available (e.g., code repositories or supplemental materials); otherwise, omit.
- **additionals**: optional list of extra resources with name and link pairs (e.g., documentation, gallery, or package links).
- **citation**: obtain the BibTeX directly from the publisher’s website (recommended).
  - As long as a DOI is provided, only authors, year, title, and venue are required.
  - Use [this tool](https://flamingtempura.github.io/bibtex-tidy/index.html) to standardize formatting.

### 2. Modify the Person Page :frowning_person:

The webmaster should collect the following items from each individual:

- **Headshot**: a 1x1 image **must** be named as `people-first-last.png|jpg|jpeg|gif|bmp` and uploaded to `assets/images`.
- **Personal link**: a website or LinkedIn profile.

Next, **edit** `_data/people.yml` file with an entry like:

```{yaml}
  - name: Jessica Hullman
    role: Ginni Rometty Professor
    department: Computer Science
    school: Northwestern University
    image: assets/images/people-jessica-hullman.jpeg
    link: http://users.eecs.northwestern.edu/~jhullman/
```

**Notes:**

- For **faculty / student**, include `name`, `role` (e.g., professor, PhD student, post doc, etc), `department`, `school`, `image`, and `link`.
- For **alumni**, include `name`, current `position`, and `link`.

## :computer: Developer Setup

### Prerequisites

Take a look on [this document for installing and configuring](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll) and [this document for testing](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).

### How to run it locally

1. Install Ruby. [Guide](https://mac.install.guide/ruby/12.html) If you could not open the link, try Incognito/Privacy mode or Safari browser. The followings are an overview:
2. Install Jekyll: `gem install jekyll` You might need to run this using `sudo`.
3. Run: `bundle exec jekyll serve`
