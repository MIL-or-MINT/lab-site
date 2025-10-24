# MU Collective Website

This is currently an in-progress repo for Jessica's #TODO [lab-name] site. Our lab site is built on `Jekyll` and this repo stores all components (i.e., images, paper pdf, metadata, etc.).

**If you are not a developer or not the web master of the year, you should not need a local setup and not need to access this repo.**

## Staff

Hyeok Kim - rebuilding the template :man_technologist:

Lily Ge - building the individual md files and managing the website after it is done :woman_pilot:

Fumeng Yang - writing documentation & nudging style :woman_juggling:

Dongping Zhang - standing on the shoulders of these giants and put the final nail in the coffin :hammer:

## Before You Start

During each academic year, a lab member will be appointed as the web master, responsible to update the site in a timely manner. The others lab members should send update request to the web master via the Slack channel `#logo-and-website` (e.g., @) or via DM.

The 2025 master is **Dongping Zhang**.

## How to update

For site maintaince and update, the web master should only need to touch three project directories: `_data`, `_posts`, and `assets`. After your edits, wait for a few minutes and check out [#TODO Site](#TODO TBD) and you should be able to see the updates.

### 1. Modify the Publications Page :page_facing_up:

To make changes to the `Publications` page, the web master should first collect the required assets from the main author, which includes: (1). a thumbnail, (2) a banner/teaser **with caption** (**with html adjustment/format**), (3)the abstract (**with html adjustment/format**) and (4) the paper pdf. Once these assets are collected, you should pay attention to two directories: `_posts` and `assets`.

You should start by giving each new paper a **unique**, **concise**, and **professional** ID. The following tutorial will be using `awesome-paper` an a running example ID.

#### 1.1 Rename and Upload the Paper Assets to `assets/`

1. The **thumbnail** works the best to have a 5:3 aspect ratio and width less than 300px to best appear in the website (ideal size: 200px by 120px). You **must** name it as `paper-thumb-awesome-paper.png|jpg|jpeg|gif|bmp` and upload it to `assets/images/`.
2. The **banner/teaser** should have its width be less than 1200px. On mobile devices, the image will be scaled to a width less than 400px, so try to avoid using too small details or letters. You **must** name it as `paper-banner-awesome-paper.png|jpg|jpeg|gif|bmp` and upload it to `assets/images/`.
3. The **paper PDF** **must** be named as `yyyy-awesome-paper.pdf` and upload it to `assets/papers/`.

#### 1.2 Create/Modify a `md` file to `_posts/`

The `_post` dir stores different `md` files, each of which serves as the entry to render unique paper page. To add a new paper, you create a new `md` file in `_post` and **must** name it as: `yyyy-mm-dd-[awesome]-[paper].md`. The month and date aren't important and you can use ascending numerical values for easier ordering of files (e.g., 2025-01-01, 2025-02-01, etc.).

A toy example below demonstrate the content of the `md` file. You can copy it as your template file. **Please read the example carefully before editing to make sure formatting is consistent and professional**.

```{yaml}
---
layout: paper
category: paper
title:  ["Copy and paste the paper title"]
authors: ["Author 1, Author 2, Author 3 -- pay attention to the formatting: do not add an "and" before the last author"]
venue: ["The Lucky Conference/Journal"]
thumb: ["assets/images/paper-thumb-awesome-paper.png"]
banner: ["assets/images/paper-banner-awesome-paper.png"]
caption: ["The caption for the banner/teaser."]
pdf: ["assets/papers/yyyy-mm-dd-awesome-paper.pdf"]
bestPaper: [true]
honorable: [false]
github: ["github.com/awesome"]
supplementary: ["https://osf.io/awesome/"]
additionals:
  - name: ["Gallery"]
    link: ["https://awesomepaper.com"]
  - name: ["Package"]
    link: ["https://github.com"]
  - name: ["Documentation"]
    link: ["https://documentation.com"]
  - name: ["Online Editor"]
    link: ["https://editor.com"]
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

Some clarifications:

- **author**: pay attention to the formatting and do not add an "and" before the last author.
- **bestPaper** and **honorable**: falg it as true or false. If the paper has no award, you can omit.
- **github** and **supplementary**: most paper will include github/supplemental materials, but can omit if none.
- **additionals**: additional links and a name to show in nested list format (e.g., package link or documentations with link). You can omit if none.
- To get citation: access the original publisher's website to get the Bibtex (strongly recommended).
  - As long as you have DOI, details other than authors, year, title, venue are not required.
  - For Bibtex, use [this tool](https://flamingtempura.github.io/bibtex-tidy/index.html) to standardize.

### 2. Modify the Person Page :frowning_person:

The web master should collect the following asset from the individual:

- A 1x1 headshot **must** be named as `people-first-last.png|jpg|jpeg|gif|bmp` and uploaded to `assets/images`.
- A personal website link (or LinkedIn)

Then, you need to **edit** `_data/people.yml` file. A toy example below demonstrate the content.

```{yaml}
  - name: Jessica Hullman
    role: Ginni Rometty Professor
    department: Computer Science
    school: Northwestern University
    image: assets/images/people-jessica-hullman.jpeg
    link: http://users.eecs.northwestern.edu/~jhullman/
```

Some clarifications:

- For a faculty/current student, you should provide their `name`, `role` (professor, phd student, post doc, etc), `department`, `school`, `image`, and website url (`link`).
- For alumni, you should provide their `name`, current `position`, and website url (`link`).

## How to update (for developer)

### Prerequisites #TODO

Take a look on [this document for installing and configuring](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll) and [this document for testing](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).

### How to run it locally #TODO

1. Install Ruby. [Guide](https://mac.install.guide/ruby/12.html) If you could not open the link, try Incognito/Privacy mode or Safari browser. The followings are an overview:
   a. `brew install ruby-install chruby`.  
   b. `ruby-install -V` At the end of installation, there are two lines `source /usr/local/...`.  
   c. `open -e ~/.zshrc` and add the two lines from the above as well as `chruby ruby-3.1.2` This is the version we are going to use.
   d. Restart your terminal and run `ruby-install ruby 3.1.2`.  
   e. It takes a few minutes and you confirm the version of ruby 3.1.2 by running `ruby -v`. If not, try to open a new Terminal.
2. Install Jekyll: `gem install jekyll` You might need to run this using `sudo`.
3. Run: `jekyll serve`
