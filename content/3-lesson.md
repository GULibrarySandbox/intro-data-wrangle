---
title: Lesson 1
nav: true
---
# The Layout of OpenRefine

OpenRefine displays data in a tabular format. Each row will usually represent a 'record' or 'observation' in the data, 
while each column represents a type of information or 'variable'. This is very similar to how you might view data 
in a spreadsheet or database. As with a spreadsheet, the individual bits of data or 'values' live in 'cells' at the intersection 
of a row and a column. OpenRefine displays only a limited number of rows of data at one time. Ten is the default.

However, the program is working on ALL rows - the limit of the number of rows displayed saves memory being wasted.

You can adjust the number of rows displayed by choosing between 5, 10, 25 and 50 at the top left of the table of data. 
You can navigate through the records by using the previous/next/first/last navigation options at the top right of the table of data.

### Working with data in OpenRefine

Most options to work with data in OpenRefine are accessed from drop-down menus at the top of the data columns. 
When you select an option in a particular column (e.g., to make a change to the data), it will affect all the 
cells in that column. If you want to make changes across several columns, you will need to do this one column at a time.

###  Rows and Records

OpenRefine has two modes of viewing data: 'Rows' and 'Records'. At the moment we are in Rows mode, 
where each row represents a single record in the data set - in this case, a respondent's survey answers. 
In Records mode, OpenRefine can link together multiple rows as belonging to the same Record. 
This is useful when working with `xml` files, MARC records, as well as `csv` files. We will see an example of this later.

### The sample dataset

We will be using open data from Transport & Main Roads obtained from the Queensland, Australia government's [open 
data portal](https://data.qld.gov.au). The original dataset presents 17 years of traffic accidents, their location, 
type of accident, level of injury, and other features, with over 300,000 observations.  

The data used in this lesson is a smaller four-year subset and has had changes made for training purposes.

### Saving projects

Projects are saved automatically as you work on them,  so there is no need to save copies as you go along. 
To open an existing project in OpenRefine, click **Open Project** from the main OpenRefine screen (in the left-hand menu). 
When you click this, you will see a list of the existing projects and can click on a project's name to open it.







# Create Lesson Content

Edit the lesson Markdown files to create content pages.

[Markdown](https://daringfireball.net/projects/markdown/) is a standard to [simplify writing](https://evanwill.github.io/_drafts/notes/writing-markdown.html) content for the web. 
[GitHub markdown flavor](https://help.github.com/articles/basic-writing-and-formatting-syntax/) can be used any where on GitHub and in Jekyll.
The basics are intuitive, you can learn in about a minute!
See [Markdown in a Minute](https://evanwill.github.io/_drafts/notes/markdown-minute.html) to get started.

When creating content pages:

- create/edit content pages in the `content` directory.
- to include a page in the nav, add `nav: true` to the file's yml front matter.
- the `title:` value will appear in the nav, sorted in the order of filenames. For simplicity use leading numbers in the lesson page filenames to create correct order.
- the default layout does not add `title` to the page, so that it can be a short for the nav. So add a title in the Markdown content.

## Components Includes

`workshop-template-b` contains a series of [Liquid "includes"](https://jekyllrb.com/docs/includes/) to add basic [Bootstrap components](https://getbootstrap.com/docs/4.1/components/) to your Markdown content.
Examples below demonstrate the includes.

--------

#### Figures 

`{% raw %}{% include figure.html img="uidaho-workshop.jpg" alt="workshop scene" caption="Library workshops!" width="75%" %}{% endraw %}`

{% include figure.html img="uidaho-workshop.jpg" alt="workshop scene" caption="Library workshops!" width="75%" %}

----------

#### Alerts

`{% raw %}{% include alert.md text="This is a Bootstrap [Alert](https://getbootstrap.com/docs/4.1/components/alerts/)" align="center" color="success" %}{% endraw %}`

{% include alert.md text="This is a [Bootstrap Alert](https://getbootstrap.com/docs/4.1/components/alerts/)" align="center" color="success" %}

-----------

#### Link Buttons 

`{% raw %}{% include button.md text="Bootstrap Docs" link="https://getbootstrap.com/docs/4.1/components/buttons/" color="info" %}{% endraw %}`

{% include button.md text="Bootstrap Docs" link="https://getbootstrap.com/docs/4.1/components/buttons/" color="info" %}

---------

#### Cards

```{% raw %}
{% capture text %}
1. Can add more complex text using markdown.
2. Use a Liquid capture to create the text.
3. It magically becomes a [Bootstrap Card](https://getbootstrap.com/docs/4.1/components/card/).
{% endcapture %}
{% include card.md text=text header="Example Card" title="Title example" img="uidaho-workshop.jpg" %}{% endraw %}
```

{% capture text %}
1. Can add more complex text using markdown.
2. Use a Liquid capture to create the text.
3. It magically becomes a [Bootstrap Card](https://getbootstrap.com/docs/4.1/components/card/).
{% endcapture %}
{% include card.md text=text header="Example Card" title="Title example" img="uidaho-workshop.jpg" %}

------------

#### Modal

`{% raw %}{% include modal.md button="Try Me" color="success" title="Example Modal" text="This is a modal, with little text." %}{% endraw %}`

{% include modal.md button="Try Me" color="success" title="Example Modal" text="This is a modal, with little text." %}
