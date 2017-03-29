# 4. Forking

You have write access to the repository on GitHub because you are part of the
uconn-maglab organization. In most cases, you will not have write access to
others' repositories. If you want to work on them, you have to make a **fork.**

## Make a fork

Go to this repository on GitHub and click Fork in the upper right. This will
make a copy of the repository on your account.

On your fork, click the Clone or Download button and copy the URL.

In a forked repository, the convention is to name the remote version of your
fork "origin" and the original one "upstream." This way, you can push and pull
like normal to origin, and pull in changes made to the main version
occasionally.

So we need to change the remotes of your local repository. Go over to GK.

On the left bar under Remote, right click on origin and select "Edit origin."

Paste the URL you copied from your fork into both the Push and Pull boxes.

Now, we need to add upstream. Hover over the Remote header and click the green
"+" button. You may be able to find it in the list of GitHub repos, otherwise
go grab the URL from the original like you did for your fork. Name it upstream.
