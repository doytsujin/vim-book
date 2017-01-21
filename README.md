# VIM - Because you are worth it

# Conventions
Markdown reference:
https://learnxinyminutes.com/docs/markdown/
# Introduction
This book is intended for programmers, system administrators or writers
that use the tex language.

You have many choices when you start programming and the easy to start
is using and IDE. For example, if you are a Python programmer, you
may want to use Jetbrains Pycharm. That's an awesome product. 
Jetbrains will target each type of language with a separate IDE. It means
that if you want to switch from Python to Javascript, then you need another
IDE.

Vim is the master of all trades. Basically, you can use Vim to master all kinds
of tasks ranging from basic workflow edition for content writers,
advanced programming, network administration etc...

In some way, all modern IDEs will provide you with Docker integration, ssh
command line tools, shell window etc...

They just copy Vim and Emacs. That's why these tools are great. Demonstration done.


#Installion and configuration
##Linux
Is natively installed.

##MacOS
Natively installed.

##Windows
Vi and Vim does not come natively on Windows.

##Useful environment variables

`$VIMRUNTIME`
If you are on Linux on MacOS, typing `:echo $VIMRUNTIME` will tell you which
Vim binary your system is currently running. In my case, it gave `/usr/share/vim/vim74`.

#Resources
A collection of packages:
http://vimawesome.com/plugin/vim-markdown-sad-beautiful-tragic

https://learnxinyminutes.com/docs/vim/

Vim's internal documentation: http://vimdoc.sourceforge.net/htmldoc/usr_41.html

IBM's tutorial on Vim Scripting: http://www.ibm.com/developerworks/linux/library/l-vim-script-1/index.html

#Vim modes
Normal mode
Insert mode
Visual mode
...

#Editing
https://learnxinyminutes.com/docs/vim/

`h` move left one character

`l` move right one character

`j` move one line down

`k` move one line up

`w` move one word right

`$` to go to end of line

`0` to go to the beginning of line

`gg` to go to the beginning of the file

`G` to go to the end of the file

`50%` go to the middle of the file. **Warning: do not type the semi-column :**.

You can access all the motion help by typing `:h up-down-motions`.


#Buffers


#Window management

Q: what is the difference with buffers? Can I work on the same file with buffers
as I would do with windows?

Windows are views on the same file.

The most important thing to know before working with Vim windows is how to 
navigate between them conveniently with the keyboard only.

The command is `<ctrl-w>`, this will allow you to jump from one window to the
other.

Opening split windows horizontally: `sp`. The same window will be split horizontally in two.
You can split vertically with `vs`.
It's very useful if you work on two different parts of the same file and 
you can't display everything on the same page. For example, if you write a 
report and want to write on a conclusion while reviewing the introduction.

You can scroll the active window while the other part remains fixed and
vice-versa.

It's very useful if you want to keep a folded version of a file and display
just one unfolded section of it the below window.

A window can be split almost infinitely in a recursive way. Golden section.

While in normal mode, you can resize the active window with the following
commands:

* `<ctrl-w> +`: increases the window height by one row.

* `<ctrl-w> -`: reduces the window height by one column.

* `<ctrl-w> >`: increases the window width by one column.

* `<ctrl-w> <`: reduces the window with by one column.

#Exploring
##nrtree
Native Vim system.

`:Explore`

`:SExplore`

`:VExplore`

##NERDTree

#Look and feel customization
If the native look and feel of Vim is rather sad, you can change it easily.
A list of installed color schemes can be found here (TODO).
Then, `:colorscheme <scheme_name>` will change the current color scheme.

If you want to use this scheme permanently, just add it to your configuration
file, `.vimrc`, in our case:

`:let colorscheme <scheme_name>`.


Color schemes
Fonts

Color scheme for Sublime users.
 
##How to create a color scheme

#Using Git

Edit your .gitconfig file
`:e ~/.gitconfig`

##Git refresher
Shortly explains git concepts like staging, commit, push, local and remote
repositories.

More information here: http://product.hubspot.com/blog/git-and-github-tutorial-for-beginners.

##Git gutter
git clone https://github.com/airblade/vim-gitgutter`.

##Fugitive
Source: https://github.com/tpope/vim-fugitive

##Installation

###Useful commands
###Staging 
Instead of calling `git add %` or `git add <file>`, simply use `:Gwrite`.

###Managing branches
####Create a new branch
####Merge branches
####Delete a branch

###Revert 
with `:Gread`.

###Commit
Once you have staged your modifications, just run `:Gcommit`.
This will open a new buffer, enter your message, save it and close the buffer
with `:wq` for instance. This will commit your file in your local repository.

###Exploring the history of a git respository
Explain what is the **Quickfix list**.


* `:Glog`: loads all previous revisions of the **current** file into the quickfix list
* `:Glog -10`: loads the last 10 previous revisions of the **current** file
* `:Glog -10 --reverse`: loads the last 10 previous revisions of the **current** file in the reverse order

Browsing past commits
* `:Glog --`: ...
* `:Glog -- %`: ...

Searching the working tree with `Ggrep`: this command is a wrapper to `git grep`.

* `:Ggrep`

Searching branches, tags and commits.

Searching for text in a commit message.

###Further readings

###Open Github
If your project is on github `:Gbrowse` will open your browser on the current 
file of your project, otherwise...

#Vimscript

##Variables
http://andrewscala.com/vimscript/

##Data types

##Loops and conditionals

##Functions

#Writing plugins

##Choosing a plugin management system

#TMux

##Installation

##Configuration

#Gems

##Cheatsheet

##Commands useful for administrators

Display the number of line in an opened file: `:echo line('$')`.

Working remotely with `ssh` and `scp`.

##Vim for Python developpers

How to configure Vim like a Python IDE.
##Vim for data analysts
How to configure Vim for data analysts.

##Vim for Javascript developpers
How to configure Vim for Javascript and Node.js developpers.

##Vim for Docker

##Vim for Nginx
