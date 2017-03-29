# 1. Meet GitKraken

GitKraken in a GUI (graphical user interface) tool for Git. It looks
complicated, but if you're familiar with the Git workflow, it can make things
a lot smoother.

## Clone this repository

First, you'll want to have this repository on your computer.

Open GitKraken and click on the folder icon in the upper left part of the
screen.

This will open the "Repository Management" window with three options on the
left bar: Open, Clone, and Init. Since you will be making a local copy of an
existing remote repository, you will want pick *Clone*.

Assuming you are part of the uconn-maglab GitHub organization, you will be able
to find this repository under the GitHub.com tab. Where it says "repository to clone,"
either start typing "git-better" or select it from the list.

Where it says "where to clone to," browse for the folder where you want to put
this repository (it will make a new subfolder for the repo), or type the path
in manually (note: do not use `~/` notation; this will create a folder called
`~` in your home directory).

Then hit "Clone the repo!"

When it is done cloning, there will be a message at the top of the window
asking if you want to switch to the repository now; click this button.

## README and LICENSE

Among the first things you should notice in a repository are the README and the
license.

### The README

Most projects have a README. This file is displayed on the home page of
a GitHub repository. It gives the visitor (and potential contributor) important
information, such as the purpose of the project, the language(s) used in its
development, how to obtain the project (whether you can download a packaged
version or if you have to build it from source), what to know when
contributing, and licensing information.

The README can be any kind of text file (e.g., `.txt`, `.md`, `.rst`), but due to
GitHub's fancy Markdown rendering capabilities, Markdown is the most common.

The README should be the first place you look when you have questions about how
to go about setting up someone else's project. Likewise, any projects you
maintain should have an up-to-date README with all the necessary information in
it. It may take time to get the hang of what to put in a README, but you can
get a good idea by looking at other projects.

### The License

Licensing is extremely important, but luckily it's also pretty easy to
understand an to do for your own work.

By default, everything you create is copyrighted to you with all rights
reserved. That means no one is permitted to modify or distribute it without your
express permission.

When you are sharing your work online, you will often *want* people to have
some of these rights so that they can use your work and contribute to its further
development, or share it with others who might find it useful.

There are many licenses that facilitate sharing to various degrees.

Works of text, art, etc. might be good candidates for a [Creative Commons
License](https://creativecommons.org). The site will ask a couple questions
about your preferences on use, modification, distribution, etc. and then find
the license that matches your needs.

As you can see from the README, this tutorial is licensed under the Creative
Commons Attribution license, meaning loosely that the user can do whatever they
want as long as they provide credit.

Anything with code should use a software license.
[Choosealicense.org](https://Choosealicense.org) can help find one for you.

The two most common open source software licenses are probably the [MIT
License](https://opensource.org/licenses/MIT) and the [GNU General Public
License (GPL)](https://opensource.org/licenses/GPL-3.0). Both of these allow
people to use and modify your code as long as they give you credit. The main
difference is that the GNU GPL requires that modifications be licensed under
the same license as the original, whereas the MIT license does not have that
constraint.

An individual preference for one license or another is a matter of personal
philosophy and practical considerations. Just make sure that if you are publishing
your work, you have *some* license on it (or an explicit statement of all rights reserved),
and that if you are using someone else's work, you do so in 


## Git workflow with GitKraken

### Branching

Right now, we are all working on our own copy of the same repository. If we all
make changes to the same file and try to push those changes to the remote repo
on GitHub, we will run into a problem known as a *merge conflict.* We will get
to merge conflicts in a bit, but for now, we'll want to just avoid them. The
best way to avoid a merge conflict is to *create a new branch* for your own
work.

On the upper toolbar on GitKraken (we'll call it GK from now on), you'll see
buttons labeled Undo, Redo, Pull, Push, Branch, Stash, and Pop. *Hit Branch*.

A little box appeared at the most recent commit. Enter the name of the new
branch. You can name it for yourself to make it easy to identify when you push
it to GitHub, or you can pick something else. You should make it all lowercase.

Hit enter when you've named it. This will create the new branch and *checkout*
(switch) to it.

This new branch contains all of the history of branch master, but any new
commits will stay on this branch until you merge it with branch master (or any
other branch).

### Modifying, staging, committing, pushing

If you're still reading this file on GitHub (or the projector), you can open it
in your favorite text editor now.

You should also open the file `demo-files/add-things-here.md` in your text
editor. Add some stuff to it. Whatever you want (within reason—remember that
what you push to the repository will be public).

Then switch back to GK. On the right, you'll see `demo-files/add-things-here.md`
listed under Unstaged Files with a yellow icon. That means there are modifications
that have not yet been staged to commit.

Hover over the file and click the green button that says "Stage file." If you
have multiple modified files, you can press the "Stage all changes" button above
the Unstaged Files box.

The file should have moved to the Staged Files box.

If you're ready to commit your changes, click on the Summary box below "Commit
Message." This is where you write your commit message. If you need an extended
commit message, you can write that in the Description box below. Otherwise,
leave the Description box blank.

When you are satisfied with your commit message, hit "Commit."
