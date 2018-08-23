# Class 3 - Sept. 14th 2018
- In this first class we will:
    - 

### Required Reading (**Must be completed ahead of time**)
Practical Computing for Biologists, Chapter 6, 16 (p.309-316)

### Preparation for next class

Python scripts are generally simple text files that are executed on the command line, just like the bash shell scripts we will be generating in today's class. However, there are also GUIs available that allow for python scripts (and those written in other programming languages), to be written and executed without needing the command line. We will use this type of interactive interface for our initial introduction to Python programming next week and again, later in the class, when we learn how to use Python to generate figures. The interactive GUI we will use is called Jupyter Notebook. 

1. Install Jupyter Notebook
There are multiple ways that you can [install the Jupyter Notebook](http://jupyter.org/install), but I highly recommend installing using the [Anaconda Distribution](https://www.anaconda.com/download/). Anaconda is available for Windows, Linux and MacOS and the Jupyter Notebook is automatically installed as a part of the Anaconda distribution. For compatibility with the PCfB book, please install the Python 2.7 version of Anaconda. 

After Anaconda has been installed, open a terminal window (Mac/Linux) or command prompt (Windows) and run the following command: ```jupyter notebook```

This should automatically open the jupyter notebook within your default browser. 

### Exercises

1. If you haven't done so already, follow the instructions on PCfB p.85-88 to set up your own scripts directory and to add this directory to your system's PATH.

2. Move into "Class3\_Shell-pt2/scratch". Within this directory, you will find a file called "dummy.txt". Write and execute a simple shell script that will:
    1. Create a new directory within "Class3\_Shell-pt2/scratch" called "dummy_dir"
    2. Move "dummy.txt" into this new directory
    3. Rename "dummy.txt" to "done.txt"

Save this script within your "scripts" directory (created in exercise #1), but run the script from within "Class3\_Shell-pt2/scratch".

3. Move into "Class3\_Shell-pt2/scratch/images". This directory contains several pdf files. Using ```ls``` in combination with regular expressions within your text editor, as described in PCfB p.91-96, quickly generate a shell script that will create renamed copies of all of these pdf files within a new sub-directory called "images\_renamed". For the image files that start with "test_", the new names should omit "test\_" from the beginning of the file names and ".txt" from within the file names. For the remaining files, omit all of the name that comes prior to the '-' character.

4. Move into "Class3\_Shell-pt2/scratch/zika\_genomes". This directory contains 88 fasta files, each containing a single Zika virus genome, and each sequence containing line within the fasta files has a maximum length of 70 nucleotides. 

This directory also contains a simple python script - "wrap_fasta.py" - that changes the length of the sequence lines in a fasta file. Here is an example command that will take an input fasta and generate a new version with sequence containing lines up to 20,000 nucleotides long:

```wrap_fasta.py  input.fasta  output.fasta 20000```

    1. Copy this python script into your 'scripts' directory and make it executable.  

    2. Use a for loop to batch process all of these Zika virus genomes, using wrap_fasta.py to create new versions in which each viral genome sequence will be contained on a single line (hint: the Zika virus genome is a little less than 11,000 nucleotides long). Make sure that you do not overwrite the original versions of the fasta sequences (i.e., the output.fasta name must be different from the input.fasta name). 

5. Write a shell function called 'whiched' that will use ```which``` to obtain the full path of a script/program in your $PATH and then automatically open that file in your text editor of choice. This can be a command line editor, like ```nano```, or a GUI editor that can be invoked from the command line, like ```bbedit```. Test this function using the "dummy.txt" script from exercise #1. 

6. Example using for loops in script??? Maybe in combination with curl


## Extra fun

[Terminus game](http://web.mit.edu/mprat/Public/web/Terminus/Web/main.html)

[Command-line Murder Mystery](https://github.com/veltman/clmystery/)

Copyright (C) 2017  Jason Ladner

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.



