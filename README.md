git-bug
=======

A repo to explore a bug I think I encountered with git and OS X

#### How I found this
I don't know exactly how I found this, but I got super weird behaviour
when I was trying to do a `git reset --hard HEAD` to remove some changes to
a vendor javascript file in my directory and it wouldn't actually remove the
changes.

Turns out, I had a vendored version of the file called `datatables.js` and someone
else recently added onto develop `dataTables.js` and then presumably, my branch
got rebased off develop.

I recorded my shell executing the steps here [https://gist.github.com/hackling/a0c85e5c7165241dbe7a]
