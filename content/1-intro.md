---
title: Intro
nav: true
---
## Background
{% include figure.html img="OpenRefine.JPG" width="75%" %}

[OpenRefine](http://openrefine.org) is a [Java](https://www.java.com/en/)-based program that runs on your computer (not online).

It runs inside your Web browser, but no web connection is needed to use it, unless you want to bring in Web-based data for cleaning. Once data has been read into OpenRefine, no further connection is needed work with it.

#### Features of OpenRefine
  
- Open source collaboratively developed software (OpenRefine source code is housed on GitHub)
- A growing community of users worldwide, from novice to expert, ready to help
- Works with large datasets, i.e. those greater than 100,000 rows
- Can adjust memory allocation to accommodate larger datasets 

#### Things you can use OpenRefine for

- Identifying where data is missing
- Identifying and fixing inconsistencies in data
- Splitting columns or rows of data up into more granular parts
- Merging columns or rows of data
- Combining multiple datasets into one
- Repeating the same step many times with different data
- Opening a dataset that is too large for Excel
- Tracking changes made to data
- Changing case within a column
- Exporting the steps as a reusable script

# Introduction

One amazingly useful GitHub feature is [GitHub Pages](https://guides.github.com/features/pages/){:target='_blank'}.
It provides free static web hosting from any repository.
Gh-pages is intended to host relatively simple sites for your GitHub portfolio, project, or documentation.
Because it is free and a valuable transferable skill, this is a great option for teaching and learning.

Many organizations are using GitHub to collaboratively create and publish public workshop websites. 
For example: 

- [Programming Historian](http://programminghistorian.org/)
- [Software Carpentry](https://software-carpentry.org/), [Data Carpentry](http://www.datacarpentry.org/), [Library Carpentry](https://librarycarpentry.org/)
- this site!

{% capture text %}Note:
There are *soft* limits and guidelines for gh-pages usage: sites should be < 1GB, use < 100GB bandwidth per month, and make < 10 builds per hour.
If your site exceeds these quotas, GitHub will send you a notice asking you to modify the repository.
All content must follow the [community guidelines](https://help.github.com/articles/github-community-guidelines/), e.g. no violence, obscene sex, or illegal stuff.{% endcapture %}
{% include alert.md text=text color=secondary %}

# workshop-template-b

`workshop-template-b` is a Jekyll project to create a simple workshop website, with a [Bootstrap](https://getbootstrap.com/){:target='_blank'} theme, designed for hosting on [gh-pages](https://pages.github.com/){:target='_blank'}.

It works best for about 5 pages of instructions, plus index, all written in Markdown. 
The navigation to the main pages is exposed at top and bottom of each page for easy stepping through the lessons.

## Why?

Rather than making slides for a workshop, why not make a website? 
It's easier to write, access, share, and reuse. 
GitHub and gh-pages makes this super easy.

It is a better [Open Educational Resource](https://en.wikipedia.org/wiki/Open_educational_resources){:target='_blank'} since anyone can easily fork and adapt!
