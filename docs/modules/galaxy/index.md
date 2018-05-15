# Starting with Galaxy

## What is Galaxy?

Galaxy is a web-based analysis and workflow platform.

  * Designed for biologists
  * Easily accessible via a web page
  * Free to use
  * You can upload your own data
  * You can access shared data
  * Use common bioinformatics tools
  * Develop workflows

In this set of tutorials, we are using **Galaxy-Australia**.

* We access Galaxy-Australia by going to a web page with this address: [add address]
* However, there are many different Galaxy servers available. Some of them have a set of general tools, and some have been developed for particular analyses. You can use more than one Galaxy server but you will need to register separately for each one, and they don't share data between them. A list of Galaxy servers is [here](https://galaxyproject.org/public-galaxy-servers/).
* More information about the Galaxy project can be found [here](https://galaxyproject.org/).


The Galaxy-Australia page looks like this:

[replace with Galaxy-Au screenshot]

![galaxy overview screenshot](images/image05.png)

* <ss>Tools</ss> on the left
* <ss>Viewing</ss> panel in the middle
* <ss>History</ss> of analysis and files on the right

## Can I use Galaxy?

Yes!

* Galaxy is free to use and available for everyone.
* Australian researchers may find Galaxy-Australia particularly suited to their analysis needs as it has been developed in consultation with scientists across the country.

## How do I get started?

To use Galaxy-Australia, follow these steps:

* Open your internet browser. Use Firefox, Chrome or Safari (not Internet Explorer).
* Open a new tab.
* In the address bar, type in the address of Galaxy-Australia [add address].

[update image]

![Galaxy URL](images/image09.png)

Click on <ss>User</ss> button on the right.

[update image]

![Register or Login screenshot](images/image04.png)

- Select: <ss>User &rarr; Register</ss>
- Enter your email, choose a password, and choose a user name.
- Click <ss>Submit</ss>

- Login, and refresh the page.

- Each time you use this Galaxy server, log in to see your data and histories.
- You have [amount of storage]
- Your data will stay stored for [amount of time.]
- If you are using a different Galaxy server, you would need to register/log in to that server.

## How to use Galaxy


* Available tools are in the left hand panel. Find the tool you want or use the search bar at the top of the tools.

* Click on the tool you want to use.

* The tool interface will appear in the centre Galaxy panel. Check the settings.

* Click <ss>Execute</ss>.

* When the tool has finished, output file(s) will appear at the top of your "Current History" in the right hand panel.

* Click on the eye icon next to a file to view it.

* To access older histories, use the button at the top right of the History panel.

## Exercise 1

### Name your current history

Your "History" is in the panel at the right.

* Click on the history name ("Unnamed history")

<img src="images/name_history.png" alt="namehist" style="width: 320px;"/>

* Type in a new name, for example, "My-Analysis"
* Press Enter

### Upload a file

Your "Tools" are in the panel at the left.

* Click <ss>Get Data</ss>
* Click <ss>Upload File</ss>
* This brings up a box:

<img src="images/upload-box.png" alt="filebox" style="width: 620px;"/>


Paste in the address of a file:
<fn>https://zenodo.org/record/582600/files/mutant_R1.fastq</fn>

Then click <ss>Start</ss>.
Then click <ss>Close</ss>.

Your uploaded file is now in your current history:

<img src="images/file-hist.png" alt="filehist" style="width: 320px;"/>


What is this file?

* This file contains DNA sequencing reads from a bacteria, in FASTQ format.
* Click on the eye icon next to the file name, to look at the file contents:

<img src="images/fastq.png" alt="fastq" style="width: 620px;"/>

### Use a tool

Let's look at the quality of the reads in this file.

* In the tools panel search box, type in FastQC.
* Click on the tool "FastQC"
* This brings up a window in the centre of the screen.
* For <ss>Short read data from your current history</ss> select the FASTQ file that we uploaded.
* Leave the other parameters as they are.
* Your tool interface should look like this:

<img src="images/fastqc.png" alt="fastqc" style="width: 620px;"/>

* Click <ss>Execute</ss>.

This tool will run and the two output files will appear at the top of your history panel.

### View results

We will look at the output file called <fn>FastQC on data 1: Webpage</fn>.

* Note that Galaxy has given this file a name according to the data it used ("data 1", or file number 1 in the history) and the tool (FastQC).

* Galaxy numbers your files but these numbers are not important.

* Click on the eye icon next to the output file. The information is displayed in the centre panel.

<img src="images/fastqc-out.png" alt="fastqc-out" style="width: 620px;"/>

* This tool has summarised information about all of the reads in our FASTQ file.
* What was the length of the reads in the input FASTQ file?
* Do these reads have higher quality scores in the centre or at the ends?

## Exercise 2

### Create a new history

### Import some data

from Zenodo

e.g. 2 x fastq files

Copy this link:

<tt>add in zenodo link</tt>

change the file name

change the file type

Use a tool - e.g. Pear

View results









## Exercise 3

### Import a history from Galaxy-Au

add a simple history to Galaxy Au

import

e.g. 2 x fastq files and a reference genome







For Galaxy-Australia users, import the following history:

[add this history to Galaxy-Au]

* In Galaxy, go to the top menu bar
* Click on <ss>Shared Data</ss>

* From the drop down menu, click on <ss>Histories</ss>

[update image]

<img src="images/shared_data.png" alt="Drawing" style="width: 500px;"/>

* From the list of Published Histories, click <fn>name of history</ss>


[update image]

![published histories](images/hist.png)


* In the top right, click on <ss>Import history</ss>

<img src="images/import.png" alt="Drawing" style="width: 400px;"/>

* This history will now be in your "Current history" - the right hand pane in Galaxy.
* There should be XX files. (The number in front of the file name is not important.)

[update image]

<img src="images/currenthist.png" alt="Drawing" style="width: 300px;"/>




### Use a tool
Use a tool - e.g. freebayes


### Filter results
then filter results


### View results

View results


## Exercise 4 - Import a shared history from a link

- Click on the <ss>History</ss> cog ![cog icon](images/image02.png)
- Select <ss>Import from File</ss>

![history options](images/import_from_file.png)

- In the box called <ss>Archived History URL</ss>, paste in the link address to the Galaxy history (that you copied above).
- Click <ss>Submit</ss>
- Wait a few seconds.
- Click on the <ss>view all histories</ss> button ![histories icon](images/view_all_hist.png)
- See if the Galaxy history has been imported: it will be called <fn>imported from archive: Data</fn>
- Above that pane, click on the <ss>Switch to</ss> button.
- Then click <ss>Done</ss> (in the top left corner).
- You should now have a list of five files in your current history. We will use these for the Genomics Workshop; or see below for additional files.

![files in galaxy history](images/datafiles.png)



## Exercise 5

### Re-run a tool

with changed settings.

## Exercise 6

### Look at all your histories

create a new history

you can drag files between histories

drag some files in

back to main page with "Analyze data"


## Summary

What have we learned?

* The Galaxy interface has tools on the left, viewing pane in the middle, and a history of your data analysis on the right.
* You can create a new history for each analysis. All your histories are saved.
* Upload data from your computer or from a web address.
* You can also upload data (and analyses) by importing a history.
* Choose a tool and change any settings for your analysis.
* Run the tool. The output files will be saved at the top of your history.
* View the output files by clicking on the eye icon.
* Log out of Galaxy-Au. When you log back in, your histories will all be there.



## What's next

try:
- MB Galaxy intro tutorial [needs updating for Galaxy-Au]





## Move this stuff:

[move this stuff below into the relevant individual workshops, to import a history for each of them: ]
