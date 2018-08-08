# Class 2 - Sept. 7th 2018
- In this first class we will:
    - Learn to use the shell/terminal to interact with your computer

### Required Reading (**Must be completed ahead of time**)
Practical Computing for Biologists, Chapters 4-5

### Some basic shell configuration

#### For Mac users:
1. Open your command line interface and confirm that you are in your home directory by typing the command:
```pwd```

  The reponse should be similar to the following with 'uname' replaced with your username:
```/Users/uname```

  If you're not in the right place, or you're not sure, execute the following command:
```cd ~/```

2. If you've installed the bbedit command line tools use the following command to open your .bash_profile in bbedit:

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

#### For Linux users:
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

1. 

2. 


3. 

## Extra fun

Explore for "extra credit" or in the event that you finish all of the other exercises.

Coming Soon!

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



