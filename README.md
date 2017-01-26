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
Dim 22 jan 17:04:19 2017
Dim 22 jan 17:04:30 2017
of tasks ranging from basic workflow edition for content writers,
advanced programming, network administration etc...

In some way, all modern IDEs will provide you with Docker integration, ssh
command line tools, shell window etc...

They just copy Vim and Emacs. That's why these tools are great. Demonstration done.

What will be covered in this book:
* basic motions and command
* Customizing and Extending Vim

Learn how to be a better developper by using better tools.

##Why this book
It took me time to collect enough resources and understanding to put all the pieces I knew about Vim together.

The book I read where much too long and did not help me to start using Vim efficiently. We know the learning curve is steep, some say it's more like a wall than a slope. So this book is itended to give you all you need to use Vim quickly in an efficient way if you are a programmer or text writer.

The idea is to help you master the basics of Vim, understand how you can use Git, the command line, Docker, use resources on the network without leaving Vim. Because, this the key point if you want to be more productive.

Once this step (waypoint) is reached, you will want to understand Vim deeper, and want to program it in order to make it suit all your needs. At this point, you will enjoy working with the keyboard only, having a clear map of all the keys etc... in your mind.

#What is Vi ? what is Vim?

##In the beginning there was Vi
Vim is a **modal** editor. 

There is nothing more faster than navigating with the keyboard, except voice maybe.

Text-objects and motions.

Vim is no vintage, it's not like Pong.


##Then came Vim
Vim stands for Vi Improved. According to the official website:
Vim is a highly configurable text editor built to enable efficient text editing. It is an improved version of the vi editor distributed with most UNIX systems. Vim is distributed free as charityware. 
Quote from
http://www.vim.org/

It was written by Bram Moolenar and first released publicly in 1991.

Basically, Vim can be run from a command line interface and as a standalone application in a graphical user interface (See Vim on Windows and MacVim on MacOS).

The wholes story started when Bram Moolenar bought an Amiga computer. On Amiga, the only editor installed was a clone of Vi, called Stevie (https://en.wikipedia.org/wiki/Stevie_(text_editor)). Stevie standed for ST Editor for VI Enthusiasts and was created by Steve Thompson on June 28, 1987. You can go to its page here: http://nosuch.com/tjt/stevie/.

###Vim today and the future
Unlike any other clones of Vi, Vim is still actively developped by a large base of contributors. New features are still being developped and added every year, making it even more powerful. Besides that, the number of Vim plugins is rapidly growing.

At the moment, Vim 7.4 is the last stable version.

###Further readings
Source: https://medium.com/@jovica/the-history-of-vim-b707758fb54f#.8teveltxy.
##And other clones

##Who uses Vim?
Great developpers, example of Damian Conway, in the Perl community.

* Damian Conway
* Pascal Precht: https://pascalprecht.github.io/2014/03/18/why-i-use-vim/. Quote: "Once you get used to it, you don't want to work without it anymore". 


Image: Vim learning curve.

###My collection of tools
* MacBook pro
* oh-my-zsh
* iTerm2
* Vim

#Installation and configuration
We will cover the main three operating systems on which you will find Vim installed.

##Linux
On Linux, whatever the distribution, Vi and Vim are natively installed.

##MacOS
Natively installed.

##Windows
Vi and Vim does not come natively on Windows.

##Useful environment variables

`$VIMRUNTIME`
If you are on Linux on MacOS, typing `:echo $VIMRUNTIME` will tell you which
Vim binary your system is currently running. In my case, it gave `/usr/share/vim/vim74`.

#Resources

A big reference, Damian Conway:
https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup

To understand autocommand:
http://www.thegeekstuff.com/2008/12/vi-and-vim-autocommand-3-steps-to-add-custom-header-to-your-file

A collection of packages:
http://vimawesome.com/plugin/vim-markdown-sad-beautiful-tragic

https://learnxinyminutes.com/docs/vim/

Vim's internal documentation: http://vimdoc.sourceforge.net/htmldoc/usr_41.html

IBM's tutorial on Vim Scripting: http://www.ibm.com/developerworks/linux/library/l-vim-script-1/index.html

On **VimL** see, Benjamin Klein, The VimL Primer: Edit Like a Pro with Vim Plugins and Scripts, on Kindle.

#Vim modes
Normal mode
:q
:q
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


`H` – Move cursor to highest (top) line in file.
`M` – Move cursor to middle line in file.
`L` – Move cursor to lowest (bottom) line in file.

`w` – Move forward a word.
`#w` – Move forward a number of words. For example, 2w moves forward two words.
`b` – Move back a word.
`#b` – Move back a number of words. For example, 3b moves back three words.
`e` – Move to end of the current word.

You can access all the motion help by typing `:h up-down-motions`.

#Copying and pasting

Vi refers to the act of copying as “yanking.”

`v` – Press v and move the cursor to select a section of text.
`y` – Copy (yank) the selected text.
`p` – Paste at cursor.
`x` – Cuts the selected text. Cuts the character under the cursor if no text is selected
`r` – Type r and then type another character to replace the character under the cursor.

##Repeat and undo

`u` – Undo.
`.` – The `.` repeats the last full command.  The insert command also functions as a command here. For example, type iunicorn and press Escape. You can then use the `.` key to insert the word unicorn at the cursor.

#Search and replace

* `/<text>`: search forward 
* `?`: search backwards
* `f`: ...
* `F`: ...
* `%`: jump between the nearest (), {} or [] characters on the line

###Search a pattern in all files
VERY USEFUL: example search a pattern in all js files:

    `:vimgrep /pg/ *.js`

Source: http://vim.wikia.com/wiki/Find_in_files_within_Vim

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

###Further reading
Plugin to resize windows using navigation keys `h`, `j`, `k`, `l`. Launch with `ctrl+E` or `:WinResizerStartResize`.  
https://github.com/simeji/winresizer

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

#Commentary
Use vim-commentary. Will detect the type of the file and add the corresponding commentary.

* `gc {motion}`: comment or uncomment lines that motion moves over
* `gcc`: comment or uncomment [count] lines
* {Visual}gc`: comment or uncomment the hightligted lines

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

###Open Github
If your project is on github `:Gbrowse` will open your browser on the current 
file of your project, otherwise...

###Further readings
We can also use the package Clam if we want to fire shell commands directly
from within Vim.
https://github.com/sjl/clam.vim.git

#Vimscript
What is Vimscript. Why and how we should use it?

##Variables
http://andrewscala.com/vimscript/

* `let`:...
* `unlet`:...
* `unlet!`:...

By default, all variables are global if it is initially defined outside a
function. Otherwise it is local to the function.

You can explicitly scope a function by prepending a specific prefix to their
name:
* `g:var`: global
* `a:var`: function argument
* `l:var`: local to a function
* `b:var`: local to a buffer
* `w:var`: local to a window
* `t:var`: local to a tab
* `v:var`: predefined by Vim

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
