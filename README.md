# Biopython

This project shows how to read, edit and analyse sequence files using Biopython.
You first need to install Biopython using ```pip install biopython```. To verify the installation worked properly type de command: ```python -c "import Bio; print(Bio.__version__)"```

Note: Depending on the version of python you are using, you may need to use ```python3``` instead of ```python``` in the command lines

## Reading Sequence Files in Biopython

The script **count_fasta.py** allow you to count the number of records in any FASTA file.

The script **count_record.py** allow you know the protein lenght of each record.

In both scripts, you only have to change the name of the file for your own file name.

To store the results in a seperate text file, you can use the following command line: ```python your_script.py > your_results.txt```

## Checking proteins start with methionine

The script **check_start_met.py** allow you to check if your protein starts with a methionine (represented as the letter "M" in the standard IUPAC single letter amino acid code) and know which ones doesn't.

## Converting a sequence file

Somnetimes you need to input a file in a specific format for an analysis. The script **convert.py** allow you to convert a GenBank file into a FASTA file. Input your file name and run the script.

## Filtering a sequence file

Sequence files can be filtered by lenght because sometimes only protein of a given lenght are required. The script **filter.py** help you doing it. In this script protein smaller than 100 amino acids will be removed but this threshold can be modified.

## Editing sequences

For some analysis, you are interested in only a subset of a bigger file. The script **edit.py** shows an example of extracting everything from a protein file except the last letter of each protein. As stated by the UPAC single letter amino acid code the ```*``` represent the termination of a protein.

## Working with Sequence Features

From a GenBank file, you might only be interested in the CDS of your sequences. The script **filter2.py** extract only the sequences that contains a CDS and output them into a seperate FASTA file.

The script **total_gene_lengths.py** gives you an example of loops to calculate the total lenght of the proteins in a sequence file.

 
