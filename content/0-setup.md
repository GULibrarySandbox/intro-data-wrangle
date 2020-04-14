---
title: Setup
nav: true
---
## Lesson setup steps
1. Download & install software
2. Download data

### 1. Get software

Note box
Installing OpenRefine on your own Windows computer may require two things:
- A JAVA install
- Moving the OpenRefine program folder to `C:\program files`. You may need administrator privileges to do this.

### Windows
- Check that you have Firefox or Chrome browsers installed and set as your default browser. OpenRefine runs in your default browser. It will not run correctly in Internet Explorer.
- Download the latest software version from [http://openrefine.org](http://openrefine.org). 
- Unzip the downloaded file into a directory by right-clicking and selecting `Extract ...`.   Name that directory something like OpenRefine.
- Go to your newly created OpenRefine directory.
- Move the folder to `c:\program files`.
- Launch OpenRefine by clicking the `openrefine.exe` file (this will launch a command prompt window, but you can ignore that and wait for the browser to launch)
- If you are using a different browser, or OpenRefine does not automatically open for you, point your browser at [http://127.0.0.1:3333/](http://127.0.0.1:3333/) or `http://localhost:3333` to launch the program.

### Windows Troubleshooting

You may also need to install Java for Windows
- Check if your Windows is 32-bit or 64-bit help via: [https://support.microsoft.com/en-au/help/15056/windows-32-64-bit-faq](https://support.microsoft.com/en-au/help/15056/windows-32-64-bit-faq).
- Select appropriate bit download
  - 32-bit via: [https://www.java.com/en/download/](https://www.java.com/en/download/) or
  - 64-bit via: [https://www.java.com/en/download/manual.jsp](https://www.java.com/en/download/manual.jsp) and 
    select Windows Offline (64-bit) version
- Choose the folder location. Save the file to `c:\program files\`
- Close all applications including the browser.
- Double-click on the saved file icon to start the installation process.
  [https://www.howtogeek.com/129178/why-does-64-bit-windows-need-a-separate-program-files-x86-folder/](https://www.howtogeek.com/129178/why-does-64-bit-windows-need-a-separate-program-files-x86-folder/) 
  
### Mac
- Check that you have Firefox or Chrome browsers installed and set as your default browser. OpenRefine runs in your default browser. It will not run correctly in Internet Explorer.
- Download latest software version from [http://openrefine.org](http://openrefine.org)
- Drag icon into `Applications folder`
- Doubleclick to launch OpenRefine
- If you are using a different browser, or OpenRefine does not automatically open for you, point your browser at [http://127.0.0.1:3333/](http://127.0.0.1:3333/) or `http://localhost:3333` to launch the program.
  
### MAC Troubleshooting
- If OpenRefine doesn’t open due to security settings go to:
  - `System Preferences> security & privacy >` see message re: OpenRefine
  - select Open anyway

### Linux
- Check that you have Firefox or Chrome browsers installed and set as your default browser. OpenRefine runs in your default browser. It will not run correctly in Internet Explorer.
- Download the latest software version from [http://openrefine.org](http://openrefine.org). 
- Unzip the downloaded file into a directory. Name that directory something like OpenRefine.
- Go to your newly created OpenRefine directory.
- Launch OpenRefine
-Type `./refine` into the terminal within the OpenRefine directory
- If you are using a different browser, or OpenRefine does not automatically open for you, point your browser at [http://127.0.0.1:3333/](http://127.0.0.1:3333/) or `http://localhost:3333` to launch the program.

#### Getting the data for the lesson

Download the `QLDtrafficAccidentsOpenDataVer1.csv` dataset from this [website](https://research-storage.griffith.edu.au/owncloud/index.php/s/NphyCS2OvSIZe8E)
to your `Downloads` folder. We will then import that data into OpenRefine.

Alternately, when you launch OpenRefine, you can import the data directly from a Web address using this link [https://raw.githubusercontent.com/stapletonsl/ClassData2020/master/QLDtrafficAccidentsOpenDataVer1.csv](https://raw.githubusercontent.com/stapletonsl/ClassData2020/master/QLDtrafficAccidentsOpenDataVer1.csv)

## Getting help

### Online

You can find out more at the [OpenRefine](http://openrefine.org) website and check out some great introductory videos. These videos and others on OpenRefine can also be found on YouTube - use the search term 'OpenRefine'.

There is a [Google Group](https://groups.google.com/forum/#!forum/openrefine) that can answer a lot of beginner questions and problems.

### At Griffith University

Help is available at Griffith [Hacky Hour & Library Researcher Support](https://hackyhourgriffith.wordpress.com/) sessions, Thursdays between 2-3pm alternating weeks at Gold Coast and Nathan campuses.  Grab a free coffee and we can help you.

[NEXT -->](data-wrangling-intro-for-hass-2.md)





