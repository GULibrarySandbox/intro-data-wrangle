---
title: Scripts
nav: true
---
# Use scripts to automate processes

A script is a series of programming steps to automate the execution of tasks.

### How OpenRefine documents changes made to data

As you conduct your data wrangling, OpenRefine saves every change you make to the dataset. 

{% capture text %}Note:
OpenRefine makes and uses a copy of your raw dataset and this original raw dataset remains unchanged.{% endcapture %}
{% include alert.md text=text color=secondary %}

These changes are saved in a format known as [JSON](https://en.wikipedia.org/wiki/JSON)(JavaScript Object Notation). You can export the JSON script and apply it to other data files. If you had 20 files to clean, and they all had the same type of errors (e.g., misspellings, leading white spaces) and all files had the same column names, you could save the JSON script, open a new file in OpenRefine, paste in the script, and run it to apply the changes to the new dataset. This gives you a quick way to clean all your related data.

{% capture text %}
- Open  `Undo / Redo`  tab
- Select  `Extract ...`

Currently all the operations you have made to the dataset are highlighted within the script window.

- Select the steps that you want to apply to other datasets by using the `check boxes`.
- `Copy` the code from the right-hand panel and `paste` it into a text editor (like *NotePad* on Windows or *TextEdit* on Mac). 
- Save it as a plain text file
  - in *TextEdit*, do this by selecting  `Format > Make plain text` 
  - and save the file as a  `.txt` file.{% endcapture %} {% include card.md header="Activity - save the data wrangling steps as a script" text=text %}

### Import a script to use with another dataset

Let's practise running the script you just created on a new dataset. We'll test this on an raw, uncleaned version of the dataset we've been working with.

{% capture text %}
Create a new project in OpenRefine using the  `QLDtrafficAccidentsOpenDataVer1.csv`  dataset you downloaded at the start of the workshop.
- Click on OpenRefine Symbol (top left-hand corner of screen), to open the menu page
- select  `Create Project`  tab
- select  `Get data from this Computer` tab >  `browse`  button
- browse to select the file `QLDtrafficAccidentsOpenDataVer1.csv` you saved to your `Downloads` folder.
- either click `Open` or double-click on the filename to import it into OpenRefine.
- click  `Next`
- give the project a different name 
- select  `Create Project`
- click the  `Undo / Redo`  tab (left-hand menu) >  ` Apply`
- paste in the contents of  `.txt`  file you saved.
- click  `Perform operations`  button{% endcapture %} {% include card.md header="Activity - import and use a script on another dataset" text=text %}

The dataset should now be the same as your other cleaned dataset.

For convenience, we used the same dataset.  You could use this process to clean related datasets.

For example, you could apply your changes to data that you had collected over different time periods or data that was collected by different researchers (provided everyone uses the same column headings).

The data in this file was generated from a database, so the column headings are pretty much guaranteed to be the same. 

----

# Save and close a project

By default, OpenRefine saves your project continuously. To close OpenRefine close the *browser tab* and the *terminal window*.  

To find a saved project, open OpenRefine and select  `Open Project`  tab, a list of projects will be available to select and open.

# Export features

In OpenRefine you can export the cleaned data or the entire project. Exporting the project as a whole means you are saving the data and all the information about the cleaning and data transformation steps you have done. 

You can export your cleaned data, with different file formats, for use in other tools for analysis.

{% capture text %}
- Click  `Export`  in the top right and select the file type for the data export. Tab-separated values (`tsv`) or Comma-separated values (`csv`) are good choices, as they are non-proprietary, but can easily be opened in programs like Excel, R, Python or the Unix shell.

Any exported file will be saved to your default  `Download`  directory.{% endcapture %} {% include card.md header="Activity - export cleaned data" text=text %}

You can also export project files as a whole. This is helpful if you wanted to send your raw data and cleaning steps to a collaborator, or share the information as a supplement to a publication.

{% capture text %}
- Click the  `Export`  button in the top right and select  `Export project`.

A  `tar.gz`  file will download to your default `Download` directory. Depending on your browser, you may have to confirm that you want to save the file. 

The downloaded  `tar.gz`  file is a folder of files which have been compressed. *Linux* and *Mac* machines will have software installed to automatically expand this type of file when you double-click on it. 

For *Windows-based* machines, you may have to install a utility like *7-zip* to expand the zip file.{% endcapture %} {% include card.md header="Activity - export a project" text=text %}

After you have expanded the file, look at the files that appear in this folder. What files are here? What information do you think these files contain?

> **Solution**

> - a history folder which contains a collection of zip files. Each of these files itself contains a `change.txt` file. 
> These `change.txt` files are the records of each individual transformation that you performed on your data.

> - a data.zip file. When expanded, this zip file includes a file called `data.txt` which is a copy of your raw data. You may also see other files.


### Going Further

Look at the other options on the Import screen - try changing some of these options and see how that changes the  `Preview`  and how the data appears after import.

Do you have access to JSON or XML data? If so, the first stage of the import process will prompt you to select a 'record path' - that is, the parts of the file that will form the data rows in the OpenRefine project. 
