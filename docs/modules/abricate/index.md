# Finding antibiotic-resistant genes

In this tutorial we will find antibiotic-resistant genes in a bacterial genome.

<fn>**New to Galaxy?** First try the [introduction](../galaxy/index.md) and then learn some [key tasks](../intro/index.md)</fn>

## Get data

* Log in to your Galaxy instance (for example, Galaxy Australia, [usegalaxy.org.au](https://usegalaxy.org.au/)).

* Create a new history for this analysis.


* In a new browser tab, go to this webpage: *http://doi.org/10.5281/zenodo.582600*
* Find the file called <fn>mutant_R1.fastq</fn>
* Right click on file name: select "copy link address"
* In Galaxy, go to <ss>Get Data</ss> and then Upload File
* Click <ss>Paste/Fetch data</ss>
* A box will appear: paste in link address
* Click <ss>Start</ss>
* Click <ss>Close</ss>
* The file will now appear in the top of your history panel.


<!--
##Import data

- Go to your Galaxy instance.
- Set up a new History for this Activity.
    - In the History panel, click on the cog icon, select <ss>Create New</ss>.
    - A new empty history should appear; click on <fn>Unnamed history</fn> and re-name it (e.g. AMR genes).

    ![Galaxy new history](images/galaxy1.png)

- Import an assembled genome (or use one from your history).
    - Copy this URL for a previously-assembled genome:  <tt>https://swift.rc.nectar.org.au:8888/v1/AUTH_377/public/Microbial_tutorials/SPAdes_contigs.fasta</tt>
    -  From the Galaxy tool panel, click on <ss>Get Data &rarr; Upload File</ss>  
    -  Click the <ss>Paste/Fetch data</ss> button  
    -  Paste the URL into the box.
    -  Click the <ss>Start</ss> button.  
    -  Once the progress bar reaches 100%, click the <ss>Close</ss> button  
    - The file will now upload to your current history.
    - Re-name it with the pencil icon to <fn>contigs.fasta</fn>.
-->


## Find antibiotic-resistant genes

- We will use the tool called [ABRicate](https://github.com/tseemann/abricate) to find antibiotic-resistant genes in the (draft) genome.
- ABRicate uses a [database](https://cge.cbs.dtu.dk/services/data.php) of these genes called [ResFinder](https://cge.cbs.dtu.dk/services/ResFinder).

In the tools panel, go to <ss>NGS Analysis: NGS Annotation: ABRicate</ss>.

- For <ss>Select fasta file</ss> choose <fn>contigs.fasta</fn> (or the name of your own assembly file.)
- Click <ss>Execute</ss>.

There is one output file. Click on the eye icon to view. It should look like this, although likely with a different number of rows.

- This shows a table with one line for each antibiotic-resistant gene found, in which contig, at which position, and the % coverage.

![abricate results](images/abricate.png)

In the output from Abricate, column 5 has the list of the antibiotic-resistant gene names. Some of these may be complete, exact matches, and some may have a gap/mutation in their sequence which can affect whether that protein is actually expressed.

To find out more about what type of AMR genes these are, you can search [Genbank](https://www.ncbi.nlm.nih.gov/gene/) with the gene name (e.g. aadD).


## What's next?

To use the tutorials on this website:

* &#8592; see the list in the left hand panel
* &#8598; or, click the **menu button** (three horizontal bars) in the top left of the page

You can find more tutorials at the Galaxy Training Network:

* [http://galaxyproject.github.io/training-material/](http://galaxyproject.github.io/training-material/)
