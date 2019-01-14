# Reference genomes

How to get a reference genome into Galaxy?

* In a web browser, go to [https://www.ncbi.nlm.nih.gov/assembly/](https://www.ncbi.nlm.nih.gov/assembly/)

* Enter the taxon into the search bar.

* For example, enter *Mycoplasma synoviae*
* Choose the assembly you want, for example, *ASM314756v1*
* Under the <ss>Assembly Definition</ss>, click on the GenBank sequence ID, for example, *CP021129.1*
* In the top right, click on <ss>Send to</ss>
* For <ss>Choose Destination</ss> select *File*
* For <ss>Format</ss> choose *FASTA*
* Click <ss>Create File</ss>
* The file will download locally.


* In Galaxy, go to <ss>Get Data</ss> and choose <ss>Upload File</ss>.
* Click <ss>Choose local file</ss>
* Select the file.
* Click <ss>Start</ss>
* Click <ss>Close</ss>
* You should now have the file in the top of your current history.
* Re-name it, e.g. to *Mycoplasma_reference.fasta*

(Alternatively: request a reference genome be added to Galaxy Australia: click on the request link on the Galaxy Australia welcome page.)

How to convert this into other formats?

Tools in Galaxy may require various formats for your reference genome. For bacterial genomes, an easy way to get the required formats is to use the tool *Prokka*.

* Go to the Tool panel and search for "prokka" in the search box.
* Click on <ss>Prokka</ss>
* For <ss>Contigs to annotate</ss>: your <fn>reference.fasta</fn> file
* All the other settings can be left as they are.
* Click <ss>Execute</ss>

Prokka outputs lots of different files including a genbank, fasta and gff version of your input fasta file.
