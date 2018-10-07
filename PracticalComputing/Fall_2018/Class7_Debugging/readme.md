# Class 7 - Oct. 12th 2018
- In this first class we will:
    - Practice debugging Python scripts

### Required Reading (**Must be completed ahead of time**)
Practical Computing for Biologists, Chapters 13,16


### Exercises

For today's exercises, I've provided a set of Python scripts, all containing bugs that either prevent execution or result in unintended results. The buggy scripts have been organized into levels depending on the nature of the bugs. 

#### **Level 1**: each script containins a single bug that will prevent the script from running

    1. Exercise 1.1: rev_comp.py is a script that accepts one or more DNA sequences as arguments on the command line. The reverse complement versions of these sequences will be printed to the screen. Here is an example command:
    
    ```rev_comp.py ACTGTAGACACACCATAG```

    There are three version of this script. Each contains a single bug. Attempt to run the example command with both versions and track down the bug based on the error messages. 
    
    2. Exercise 1.2: string_replace.py replaces a list of strings within a file, each with a specified replacement string. The target and replacement strings are provided as a tab-delimited file (e.g., "names_to_replace.txt"). You also need to provide the input file and a name for the output file. Here is an example command:
    
    ```string_replace.py -i infile.txt -o outfile.txt -s names_to_replace.txt```

    There are three version of this script. Each contains a single bug. Attempt to run the example command with both versions and track down the bug based on the error messages. 

    3. Exercise 1.3: fasta2phy.py is a script that converts a fasta formatted alignment file to a relaxed phylip formatted file. Here is an example command:
    
    ```./fasta2phy.py -f lassa_seqs.fasta```

    There are three version of this script. Each contains a single bug. Attempt to run the example command with both versions and track down the bug based on the error messages. 


## Extra fun

Coming soon!

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



