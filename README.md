[![MIT License][license-shield]][license-url]
<!-- LOGO -->
<h4 align="center">A Jekyll Theme by DeerRIDER.</h4>
<p align="center">
  <a href="https://github.com/akiritsu/pRoJEct-VeXEd">
    <img src="src/assets/img/favicon.png" alt="Logo" width="275" height="275">
  </a>
</p>
<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.
<!-- TABLE OF CONTENTS -->
## Table of Contents
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Personalize and Customize](#personalize-and-customize)
    - [_config.yml](#_configyml)
    - [Collections](#collections)
    - [Writing](#writing)
    - [Comment](#comment)
    - [Test locally](#test-locally)
    - [Front Matter](#front-matter)

## Getting Started

### Prerequisites
* rubygems

The installation of gem is depend on your operating system. Alternatively, you can download Gem through browser: [Ruby](https://www.ruby-lang.org/en/downloads/), and install rubygems manually.

```bash
# macOS

brew update
brew install ruby

# Ubuntu
sudo apt-get install ruby

# Arch
sudo pacman -S ruby

```

* bundler

```bash
gem install bundler
```
* jekyll
```bash
bundler install jekyll
```

* jekyll plugins

```bash
gem install jekyll-sitemap jekyll-feed jekyll-seo-tag jekyll-mermaid
```

### Installation

1. Fork this project on [github](https://github.com/akiritsu/pRoJEct-VeXEd), change project settings, and clone your own repository into your local disk.

```bash
git clone https://github.com/{{YOUR_USERNAME}}/{{YOUR_REPOSITORY}}.git
```

2. Change directory.

```bash
cd {{YOUR_REPOSITORY_DIR}}
```

### Personalize and Customize

#### _config.yml

Edit **_config.yml** with your own website information.

#### Collections

All your articles could be stored in this folder. You could create a new collection by creating a subfolder begin with a slash, and register the basic information in **_config.yml**. Here is an example:

```yaml
# Collections
collections:
  notes:
    output          : true
    permalink       : /:collection/:title/
    sort_by         : date
  portfolio:
    output          : true
    permalink       : /:collection/:title/
    order: # specify post order manually
      - portfolio3.md
      - portfolio2.md
      - portfolio1.md
  album:
    output          : true
    permalink       : /:collection/:title/
    sort_by         : date
```

All your articles would be shown by clicking **Archive** button in the header of your website.

#### Writing

Delete all sample collections under **./collections/**, and have fun in writing!

#### Comment

Create your own account in [Disqus.com](https://disqus.com/), and change the attribute "disqus_username" in **_config.yml**.

#### Test locally

Run command below, and access "127.0.0.1:4000" to test your website locally.

```bash
bundle exec jekyll serve
```

#### Front Matter

You can add many front matter to customize a page. For more information, visit official document: [https://jekyllrb.com/] (https://jekyllrb.com/docs/front-matter/)

```yaml
layout: post # page layout, must be one of layouts under src/_layouts
title: "Sample" # string
author: "your_name" # string
post_list: "cate" # whether to show post list under collections/_post, one of false, "cate", "date"
collection_list: true # true or false
toc: true # table of content, true or false
show_date: true # whether to show date, true or false
home_btn: true # whether to show home button, true or false
btn_text: true # whether to show button text, true or false
footer: true # whether to show footer, true or false
maximize: true # whether to show maximize button, true or false
encrypted_text: true # whether to enable encrypted text, true or false
publish: true # if you wish keep this page invisible, put false here
toc_level: 4 # the depth of toc, one of 1, 2, 3, 4, 5, 6
comment: ture # whether to show comment area
category: "sample" # string
date: 2019-5-25 # YYYY-MM-DD
excerpt: "This is excerpt." # string
abstract: "This is abstract. Abstract is blank by default." # string
```

[license-shield]: https://img.shields.io/github/license/akiritsu/pRoJEct-VeXEd.svg?style=flat-square
[license-url]: https://github.com/senyirauxa/senyirauxa.github.io/blob/master/LICENSE
