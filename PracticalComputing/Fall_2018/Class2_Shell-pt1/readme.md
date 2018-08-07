# Class 2 - Sept. 7th 2018
- In this first class we will:
    - Learn to use the shell/terminal to interact with your computer

### Required Reading (**Must be completed ahead of time**)
Practical Computing for Biologists, Chapters 4-5

### Some basic shell configuration

# For Mac users:
1. Open your command line interface and confirm that you are in your home directory by typing the command:
```pwd```

If the reponse should be similar to the following with 'uname' replaced with your username:
```/Users/uname```

If you're not in the right place, or you're not sure, execute the following command:
```cd ~/```

2. If you have installed the bbedit command line tools use the following command to open your .bash_profile in bbedit:

```bbedit .bash_profile```

Alternatively use this command to open your .bash_profile in a terminal-based text editor  

```nano .bash_profile```

3. Add the following lines of code and save your changes:

```
set -o noclobber

# For incremental search capabilities
bind '"\e[A": history-search-backward'
bind '"\e[B": history-search-forward'
```

4. Run the following command from the terminal window:

```source .bash_profile```

# For Linux users:
1. Open your command line interface and confirm that you are in your home directory by typing the command:
```pwd```

The reponse should be similar to the following with 'uname' replaced with your username:
```/home/uname```

If you're not in the right place, or you're not sure, execute the following command:
```cd ~/```

2. Open your .bash_profile in a terminal-based text editor. This command will create the file if it doesn't exist:  

```nano .bash_profile```

3. Add the following lines of code and save your changes. These will ensure that commands within .bashrc will also be run when only your .bash_profile is executed:

```
if [ -f ~/.bashrc ]; then
   source ~/.bashrc
fi
```

4. Open your .bashrc in a terminal-based text editor. This command will create the file if it doesn't exist:  

```nano .bashrc```

5. Add the following lines of code and save your changes:

```
set -o noclobber

# For incremental search capabilities
bind '"\e[A": history-search-backward'
bind '"\e[B": history-search-forward'
```

6. Run the following command from the terminal window:

```source .bashrc```


### Exercises

1. Got to [RegexOne](https://regexone.com/) and complete the 15 lesson tutorial. This website provides a nice interactive interface for playing with regular expressions.
    - Keep track of your solutions to share with the class

2. We will now start using the text editor on your computer to use regular expressions to edit text files. 
    1. Open "EBOV.phy" in your text editor.
    2. Use a series of search/replace queries to covert this phylip formatted sequence alignment into a fasta formatted file. Two commands should be sufficient. Fasta format:
     ```
     >name1
     seq1
     >name2
     seq2
     ```
    
    3. Edit regular expression to change sequence names. New names should only include the characters prior to the first underscore ('_')
    4. Edit regular expression to remove all 'N' characters from the beginning and end of each sequence

3. Open "HastingsBirdList\_2007\_.txt" in your text editor. This file contains tab-delimited information about bird species cited in the Hastings Park Conservancy in Vancouver, BC.
    1. Design a single search and replace query that utilizes regular expressions to reformat **every** line to the following format:
    ```Genus\tspecies\tG. species\tCommon Name\tStatus```
    "Status" is the column with a categorical variable including "Casual", "Rare Visitor", etc. Make sure to remove the "*" character from the beginning of the Status category, if present. 

## Extra fun

Explore for "extra credit" or in the event that you finish all of the other exercises.

[Regex Crossword](https://regexcrossword.com/)

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



