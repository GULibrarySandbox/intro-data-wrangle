---
title: Start
nav: true
---

# Creating a new OpenRefine project

OpenRefine works with a variety of file types, including tab separated (`tsv`), comma separated (`csv`), Excel (`xls, xlsx`), `JSON`, `XML`, `RDF as XML`, and `Google Spreadsheets`.

See the [OpenRefine Importers page](https://github.com/OpenRefine/OpenRefine/wiki/Importers) for more information.

### Launching OpenRefine

**Windows**: double-click on the `openrefine.exe` file. Java services will start automatically on your machine, and OpenRefine will open in your browser. Be sure to use either Chrome or Firefox, as OpenRefine does not play well with Microsoft Edge or Safari.

**Mac**: OpenRefine can be launched from your Applications folder.

**Linux**: navigate to your OpenRefine directory in the command line and enter `./refine`.

Once OpenRefine is launched in your browser, the home screen displays options to **Create Project**, **Open Project**, or **Import Project**.
You will create a project.

### If launch fails

If OpenRefine does not automatically open within your browser after launch, point your browser at `http://127.0.0.1:3333/` or `http://localhost:3333` to launch the program.
{% capture alert %}Note: Keep the terminal window hosting Java open the in the background.{% endcapture %} {% include alert.md text=alert color="warning" %}

### Creating Project

Projects can be created in a variety of ways, e.g., by uploading data from your computer or by importing it from a web address.

#### To create a project by uploading data from a local source

- Choose **Create Project**
- Select **Get data from this Computer**.
- Select **Choose Files** and browse to select the file `QLDtrafficAccidentsOpenDataVer1.csv` you saved to your **Downloads** folder.
- Either click **Open** or double-click on the filename to import it into OpenRefine.
- Click **Next**.

#### To create a project by importing the data from a Web Address

- Choose **Create Project**
- Click **Web addresses (URLs)**.
- When a text box opens, enter this address `https://raw.githubusercontent.com/stapletonsl/ClassData2020/master/QLDtrafficAccidentsOpenDataVer1.csv`
- Click **Next**.

### Data preview

OpenRefine gives you a preview to show you how it has interpreted the file you have uploaded or imported. If your data was tab- rather than comma-delimited, the preview might look strange. Be sure the correct separator is displayed in the box shown. If you have made any changes, click Update Preview (bottom left). If the wrong file is displaying, click <<Start Over (upper left).

There are options to indicate whether the dataset has column headers included and whether OpenRefine should skip a number of rows before reading the data. Ensure the first row is used to create the column headings by checking the box `Parse next 1 line(s) as column headers`

Make sure the `Parse cell text into numbers, dates,` ... box is not checked, so OpenRefine doesn't try to automatically detect numbers. Parsing in this context refers to the way the software will interpret the format of the data.

Choose **UTF8** as the method of encoding as this should convert any 'smart' formatting into plain text.

If all looks fine, click **Create Project**.

### Key Points

- Use the **Create Project** option to import new data to work on.
- You can control how data is imported b y changing options on the import screen.


The `workshop-template-b` [repository](https://github.com/evanwill/workshop-template-b) is a skeleton project. 
This [site](https://evanwill.github.io/workshop-template-b/) demonstrates the output on gh-pages, and the content pages serve as examples.

{% capture text %}
1. Fork or import the [repository](https://github.com/evanwill/workshop-template-b) on GitHub.
2. Clone to your local machine, or work on the GitHub web interface to edit files.
3. Edit the `_config.yml` with your info.
4. Edit the content pages in markdown.
5. Add images to the "images" folder.
5. Push to GitHub (or commit on the web interface).
6. In your repo's settings, activate gh-pages, using master branch.{% endcapture %}
{% include card.md header="Overview" text=text %}

## Config

Edit the `_config.yml` to get your workshop website set up.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
Pellentesque eu velit felis. 
Duis fermentum est nec mollis scelerisque. Vivamus interdum efficitur mauris, et dignissim velit egestas vitae. 
Cras dignissim sagittis varius. Pellentesque eu laoreet dui.

```
Praesent congue:
    eros = eget
    accumsan euismod
```

Praesent congue, eros eget accumsan euismod, lorem dui vulputate leo, tincidunt efficitur risus metus ut risus. 
Sed pharetra ipsum orci, eu cursus turpis semper egestas. 

> Pellentesque sodales, felis auctor auctor rutrum, velit quam interdum erat, sit amet placerat urna nisl at justo.

## Substep

Nam maximus eget orci id pretium. Pellentesque feugiat mauris eu nulla viverra consectetur. Nullam rutrum augue eget mauris accumsan, ac elementum tellus lacinia. Sed pretium aliquet tortor in ornare. Sed eget aliquet metus. Integer sed arcu turpis. Duis auctor sollicitudin semper. Cras posuere, neque nec varius cursus, massa libero sodales elit, sed tempor nibh ex sit amet nisi. Quisque consequat ante quis diam malesuada, in imperdiet tortor mattis. Aliquam erat volutpat. Morbi tortor elit, sagittis quis nibh ut, gravida cursus arcu.

{% include figure.html img="uidaho-workshop.jpg" alt="workshop scene" caption="Be sure to replace all the example values!" width="75%" %}

Ut dapibus lectus tristique efficitur dictum. Quisque efficitur ornare sagittis. Donec ex sem, volutpat quis scelerisque quis, scelerisque non neque. Vivamus convallis felis vel eros pulvinar faucibus. Aliquam finibus pretium odio a pharetra. Nullam ac commodo magna. Fusce et feugiat sem. Nunc vitae scelerisque metus. Aenean sodales placerat mi in aliquet. Curabitur pulvinar auctor mauris quis faucibus. Ut commodo imperdiet ante, at dignissim tellus ultricies ut. Donec at lacus ultrices sem vulputate semper. Donec commodo porta nunc, non tristique mi interdum quis. Phasellus rhoncus bibendum ipsum, ac malesuada augue pulvinar et. Etiam finibus lacus massa, sit amet faucibus lorem consequat sit amet. 
