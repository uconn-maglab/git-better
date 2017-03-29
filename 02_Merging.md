# 2. Merging

## Merge your work into the main branch

Now it's time to incorporate your changes back into the main branch.

In GK, find the last commit on branch master. Right click on the master tab.
Select "Merge [your-branch-name] into master."

Now checkout to master by double-clicking on its name on the left bar under
"local." Cool, all of the changes you made on your branch are in the main
branch. (**Note:** In case you're like me and learn by trying things to see
what happens, please *do not push branch master right now*.)

## Pulling from GitHub

Just as you push your commits to GitHub, you'll need to **pull** from GitHub to
get your collaborators' commits.

Press the Pull button to fetch everyone else's branches as well as the changes
I've made to master.

## Resolving merge conflicts

Remember how I said we can't all work on the same branch or else we'll run into
a merge conflict? Yeah...here we are!

Pulling is a version of merging, specifically merging a remote branch into a
local one.

If two commits have edited the same lines, Git doesn't know which lines you
want. So it aborts the merge until you resolve the conflict.

Luckily, GK makes it pretty easy to resolve a merge conflict.

Click on the file with the conflict in the right bar. This will open a page
that looks a lot like the diff page, but it has the conflicting diffs for the
two files.

Go through and check the boxes of the changes you want to keep, then hit Save
in the upper right.

Now you can commit like normal. It even gives you a ready-made commit message!

## Avoiding merge conflicts

Merge conflicts can be frustrating. The best way to avoid them is to **pull
before you make changes**. It also helps to work in a separate branch and pull
to the main branch before merging your branch into it.
