---
layout: post
title:  "Host Jekyll site on Gitlab"
date:   2018-09-28 10:10:10 +0700
categories: [Ruby, jekyll]
comments: true
---

**Contents**
* TOC
{:toc}
## How this site come into being?
It credit to Free and open-source Jekyll theme [https://agusmakmun.github.io](https://agusmakmun.github.io).

Build a Jekyll website is my primary goal, the secondary goal is to deploy it on
gitlab. Things would become easier if you know
* How to use Jekyll with bundle
* How to write `.gitlab-ci.yml` file.

## Quickstart
Customize from scratch, you just
* Build a blog with default theme. [Guide](https://jekyllrb.com/docs/)
Run `bundle exec jekyll serve` on terminal and preview on a browser.

Let the professional web developer take care of the web style. you
* Choose a theme from [jekyllthemes.org](jekyllthemes.org) or [jekyllthemes.io](https://jekyllthemes.io/).
  The formal is contributed by volunteers, and the latter is mostly in charge.

Since my idea is contents oriented blogging and leave behind the the work of
front-end, I choose the minimal theme type.
## Advanced techniques
* Automate the procedure of create a post

  Jekyll requires blog posts to be saved in files with a specific filename. `YY-MM-DD-Title.md`, which is annoying to realize manually. Automatic the process of creating a new post with rake task. [Using Rake to automatic tasks](https://www.stuartellis.name/articles/rake/)

  eg: `rake post TITLE='hello, world'`

* [Enable mathjax](http://sgeos.github.io/github/jekyll/2016/08/21/adding_mathjax_to_a_jekyll_github_pages_blog.html)

  Displaying Mathematical formula is common in the posts, here I use `Mathjax` to realize it.
*  Add Disqus to Jekyll website

   [Instructions given by Disqus](https://disqus.com/admin/install/platforms/jekyll/) is quite straightforward.

   * Add `comments: true` to Front Matter
   * Copy and paste the Universal Embed Code in the appropriate template where you'd like Disqus to load.

   * [disqus comments on jekyll show when host on  local but not when host on gitlab](https://stackoverflow.com/questions/48281060/disqus-comments-on-jekyll-show-when-hosted-on-localhost-but-not-when-hosted-on-g)


* [Add Table of Contents to Jekyll Blog](https://ouyi.github.io/post/2017/12/31/jekyll-table-of-contents.html)

  Fortunately, rendering of table of contents (TOC) is supported by kramdown, which is Jekyll 3.0.0’s default Markdown processor

## Continuous integration in Gitlab?
> GitLab offers a continuous integration service. If you add a .gitlab-ci.yml file to the root directory of your repository, and configure your GitLab project to use a Runner, then each commit or push triggers your CI pipeline.

> The .gitlab-ci.yml file tells the GitLab runner what to do. By default it runs a pipeline with three stages: build, test, and deploy. You don't need to use all three stages; stages with no jobs are simply ignored.

What Deploy means ?

If I test the site locally, and it works perfect, what is the necessity to run
on cloud to test the website.

You have witnessed that how hard developers maintain their product. They well tested their software, but there are problems on different platforms.


[7 reasons why you should be using Continuous Integration](https://about.gitlab.com/2015/02/03/7-reasons-why-you-should-be-using-ci/).

## A frequently problem you might encounter
```
Conversion error: Jekyll::Converters::Scss encountered an error while converting 'assets/css/style.scss':
                  Invalid US-ASCII character "\xE2" on line 5
```

[Someone's experience helps to answer ](http://talk.jekyllrb.com/t/how-to-deal-with--sass-converting-errors/911/2)

You got to know the principle, mechanism, rule behind how things actually work.
For instance, figure out how Jekyll organize the blog file system and what each
file used for, like the role play by `_config.yml` in Jekyll.
