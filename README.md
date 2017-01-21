# VIM - Because you are worth it

# Conventions

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

#Resources
http://vimawesome.com/plugin/vim-markdown-sad-beautiful-tragic

#Vim modes
Normal mode
Insert mode
Visual mode
...

#Editing

`h` move left one character

`l` move right one character

`j` move one line down

`k` move one line up

`w` move one word right

`$` to go to end of line

`0` to go to the beginning of line

`gg` to go to the beginning of the file

`G` to go to the end of the file

#Window system

#Tabs

#Folding
help
command is z
the mnemonic, look a z like a something that can expand and retract, like
a spring.
http://vimcasts.org/episodes/how-to-fold/

#Exploring
##nrtree
Native Vim system.

`:Explore`

`:SExplore`

`:VExplore`

##NERDTree

#Look and feel customization
Color schemes
Fonts

#Using Git

Edit your .gitconfig file
`:e ~/.gitconfig`

##Git refresher
Shortly explains git concepts like staging, commit, push, local and remote
repositories.

##Git gutter
git clone https://github.com/airblade/vim-gitgutter`.

##Fugitive
Source: https://github.com/tpope/vim-fugitive

##Installation

###Useful commands
###Staging 
Instead of calling `git add %` or `git add <file>`, simply use `:Gwrite`.

###Revert 
with `:Gread`.

###Commit
Once you have staged your modifications, just run `:Gcommit`.
This will open a new buffer, enter your message, save it and close the buffer
with `:wq` for instance. This will commit your file in your local repository.

###Open Github
If your project is on github `:Gbrowse` will open your browser on the current 
file of your project, otherwise...

#Vimscript

#Writing plugins

##Choosing a plugin management system

#TMux

##Installation

##Configuration
