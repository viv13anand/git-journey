Git is a powerful tool that
constantly keep track of every change
you make to your files, aka local.

GitHub acts as that central
online server where the entire
project lives, making it easy for
everyone to see, edit, and share updates
in one single place, aka remote.

a repository is a place where all
the versions of your files and their
complete change history are stored. 
In
the case of a local repository, it's a
specific folder on your own computer.
For a 
remote repository, it lives on a
cloud server like GitHub. 

You can think
of a repository as a digital cabinet for
your code, a secure place where Git
neatly stores every record of your work
and every change you have ever made.

---

--- how the local part works ---

In your computer, the folder where you are
working on your project is called the
working directory. 
This is where all the
action happens. You write code, create
new files, modify existing ones, and
make changes as needed. 
And when you
feel all right, this version looks good
and want to save this change. That's when
you move on to the next stage in git workflow.

Staging
process is the second phase in Git's
workflow.
Staging area is a middle
ground, a temporary space where files
sit between your working directory and
the final save in the repository.
Once
you have reviewed everything and you are
confident the work is correct, you
commit it.

Committing means permanently
saving those changes to your local
repository, locking them in as a
recorded version of your project's
history.

First, we work inside
our local working directory. Once we are
done, we stage our changes and then
commit those staged files to the local
repository.

The process of moving changes from the
working directory to the staging area is
called adding.

---

A branch in Git is like a
separate line of development where you
can work independently.

The default branch is
called main.
The main branch is your
project's central line of development.

Instead of
making changes directly on the main
branch, you create a separate
development branch where you test and
commit all your changes. 

Once everything
is stable and verified, you merge that
branch back into the main branch.

Merge
simply means combining the changes from
two branches into one.

A merge conflict
happens when the same part of the same
file has been changed differently in two
branches.
Git flags the file as having
a conflict and you will have to resolve
it manually by deciding which changes to
keep or by merging both versions
yourself.

When we send
local changes to a remote repository,
that process is called a push.   

If any changes have been made in the remote
repository that we want to bring into a
local repository, we use fetch.

When you
run git fetch, the remote changes are
downloaded into your local repositories
memory, but they won't appear in your
working directory yet. To actually
update your working directory and see
those changes in your files, you need to
run git pull.

push means
sending local changes to the remote.

Fetch means bringing remote changes into
your local repository but not merging
them yet.  

pull means fetching plus
merging. pull = fetch + merge.

The revert command is used to undo the
changes made in a previous commit. But
instead of deleting that old commit, it
creates a new one that reverses those
changes.
It cancels out
the effects of a previous commit while
keeping the project history completely
clean and traceable.

When you perform a rebase,
the base of your feature branch changes.
That means if you rebase onto main, all
the new commits from main will be applied
directly into your feature branch. 
All your feature branch commits will be
reapplied on top of them.
However,
even though git rebase is very powerful,
it's not recommended to use it on public
repositories or branches where multiple
developers are working together. 
If you
must use it, you should always inform
your team beforehand. Otherwise, it can
cause serious issues. 
The reason is that
rebase rewrites existing commit history.
even the comet ids change. So if someone
else is working on the same branch, your
rebased commits won't match their local
copies anymore and they won't be able to
pull or sync normally. Therefore, before
using rebase, make sure you fully
understand where you are applying it and
whether it could cause problems for your
collaborators.

