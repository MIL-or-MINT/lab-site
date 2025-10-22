# MU Collective Website

This is (currently) an in-progress repo for Jessica's lab site. This website is built on `Jekyll`.

## Staff

Hyeok Kim - rebuilding the template :man_technologist:.

Lily Ge - building the individual md files and managing the website after it is done :woman_pilot:.

Fumeng Yang - writing documentation & nudging style :woman_juggling:.

Dongping Zhang - standing on the shoulders of these giants and put the final nail in the coffin :hammer:.

## How to update (for everyone)

First, you should find the information you need to prepare on this page (looking for `[for everyone]` notation).

Second, you send them to the master person in the Slack channel `#logo-and-website` (e.g., @) or via DM. The 2025 master is **Dongping Zhang**.

## How to update (for the master person)

Basically, we keep everything (images, pdf, metadata, etc.) on Github. If you are not a developer, you should not need a local setup.

In sum, you only need to touch `_data`, `_posts`, and `assets`. **Hyeok: "If you are touching anything else, it means you are doing something wrong."**

After your edits, wait for a few minutes and check out [#TODO Site](#TODO TBD) and you should be able to see the updates.

### Add a [paper](https://mucollective.github.io/publications) :page_facing_up

The two folders you have to pay attention to are:

- `_posts`: This folder provides information for papers. You need to add a new `*.md` file when you want to add a paper.
- `assets`: This folder provides the actual thumbnails and PDFs.

`[for everyone]` To add a paper, you need to prepare the followings:

- **a unique ID**: say `awesome-paper` and it is published in `yyyy`. This ID is used everywhere to grab information for rendering the website.
- **a `.md` file** (see below) that will be uploaded to `_posts` : you **must** name it `yyyy-mm-dd-awesome-paper.md` The month and date aren't important. You can use any values. The master person prepares this file.
- **the paper PDF** that will be uploaded to `assets/papers/`: you **must** name it `yyyy-awesome-paper.pdf`
- **a teaser/banner** that will be uploaded to `assets/images/`: you **must** name it `paper-banner-awesome-paper.png|jpg|jpeg|gif|bmp`. The width should be less than 1200px. On mobile devices, the image will be scaled to a width less than 400px, so try to avoid using too small details or letters.
- **a thumbnail** that will be uploaded to `assets/images/`: you **must** name it `paper-thumb-awesome-paper.png|jpg|jpeg|gif|bmp`. We strongly suggest to use a 5:3 aspect ratio and width less than 300px to best appear in the website (ideal size: 200px by 120px).
<!-- The width should be less than 1200px, and we suggest to use a 5:3 aspect ratio to align with other images. (Fumeng: I hope you can follow this rule such that we don't have to run resize scripts for you!) -->
- authors, abstract, venue, year, awards
- other links you want to show and their names

#### The `.md` file

This file **must** be called `yyyy-mm-dd-awesome-paper.md` It provides entries to render a paper. Again, you must specify year like `2022-12-01-awesome-paper.md` but months and days are not important.

A toy example is below. You can copy it as your template file. (`[for everyone]` Here, you can get a sense of what information you need to prepare, but the master person will prepare the `.md`.)

```{yaml}
---
layout: paper
category: paper
title:  "This is an awesome paper"
authors: "Author 1, Author 2, Author 3"
venue: "The Lucky Conference/Journal"x
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
---

<!-- abstract -->
This is our awesome paper published at the Lucky Conference.

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

<div class="apa">
<!-- apa -->
<h4>APA</h4>
<p>APA FORMAT STRING.</p>
</div>
```

Explanation:

- **layout: paper** - this must be `paper`.
- **category: paper** - This can take more than one keyword, like `paper quant-uncerntainty`. The second keyword is used to put the paper under a research area, which you can find under `_data/research_area.yml` (the `cat` field.) If you don't know, leave it as `paper`.
- **title...pdf** - ordinary stuff. Notice that you must follow the naming style!
- (optional) **bestPaper** and **honorable** - true or false. You can also skip it.
- (optional) **github** and **supplementary** - You can also skip it.
- (optional) **additionals** - additional links and a name to show. You can also skip it.
- To get citation: access the original publisher's website to get the Bibtex (strongly recommended) and APA format (optional).
  - As long as you have DOI, details other than authors, year, title, venue are not required.
  - For Bibtex, use [this tool](https://flamingtempura.github.io/bibtex-tidy/index.html) to standardize.

Now,

- upload `yyyy-mm-dd-awesome-paper.md` to `_posts`
- upload `yyyy-awesome-paper.pdf` to `assets/papers`
- upload `paper-banner-awesome-paper.png` and `paper-thumb-awesome-paper.png` to `assets/images`

You are all set.

### Add a new [person](https://mucollective.github.io/people) :frowning_person

`[for everyone]` You need to prepare the followings:

- A 1x1 headshot named `people-first-last.png|jpg|jpeg|gif|bmp`. (Fumeng: I don't know if you want to use a gif, but it is possible?) You must follow the naming style `people-...`.

You only have to **edit** `_data/people.yml` file and upload the image to `assets/images`.

`[for everyone]` An example:

```{yaml}
  - name: Jessica Hullman
    role: Ginni Rometty Associate Professor
    department: Computer Science
    school: Northwestern University
    image: assets/images/people-jessica-hullman.jpeg
    link: http://users.eecs.northwestern.edu/~jhullman/

```

Explanation:

- For a faculty/current student, you should provide their `name`, `role` (professor, phd student, post doc, etc), `department`, `school`, `image`, and website url (`link`).
- For alumni, you should provide their `name`, current `position`, and website url (`link`).

### Edit [research area](https://mucollective.github.io/research) :mortar_board

You only need to edit `_data/research_areas.yml` file.

An example:

```{yaml}
- name: Communicating unquantified uncertainty
  category: unquant-uncertainty
  desc: We aim at communicating unquantified uncertainty.
  image:
    - "assets/images/research-image-...."
```

Explanation:

- **name** is the name to show in the list
- **category** is the catergory, which will be used to match and grab papers.
- **desc** is the description.
- **image** is the list of related images to show (suggestion: upto 2). You can list images in the YAML list format.

### Add or edit a [public release](https://mucollective.github.io/public-release) :earth_americas

`[for everyone]` You need to prepare the followings:

- URLs to your release.
- The categories of your releases: software, prototype, or something else. Examples are listed below.

There are two files `_data/prototype.yml` and `_data/software.yml`. Our suggestion is that if it is a concrete thing, then it belongs to `software`. The entry should be very much self-explanatory.

An example from `_data/prototype.yml`:

```{yaml}
- title: Cicero
  contributor: Hyeok Kim
  type: JS library
  supplement:
    - type: Gallery
      link: https://see-mike-out.github.io/cicero-supplemental/
  description: Cicero is a declarative grammar for responsive visualization transformatons.
```

An example from `_data/software.yml`:

```{yaml}
 title: ggidst
  contributor: Matthew Kay
  type: R package
  supplement:
    - type: Documentation
      link: https://mjskay.github.io/ggdist/
    - type: Code Repository
      link: https://github.com/mjskay/ggdist
    - type: CRAN
      link: https://cloud.r-project.org/web/packages/ggdist/index.html
  description: ggdist is an R package that provides a flexible set of ggplot2 geoms and stats designed especially for visualizing distributions and uncertainty.
```

### Add or edit a [talk](https://mucollective.github.io/talks) :speech_balloon

You only need to edit `_data/talk.yml` file.

```{yaml}
- title: Uncertainty visualization with tidybayes and ggdist
  year: 2021
  contributor: Matthew Kay
  venue: Bayes@Lund
  link: https://youtu.be/EtrmxMX8zWw
```

### Edit text on homepage on the top

- Text on the top left section: `_data/home_text.yml`

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
