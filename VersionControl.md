# Git Rebase, Git Squash, Git Merge


# Git Rebase:
  Git rebase is a command in Git that allows you to integrate changes from one branch onto another. It is commonly used to incorporate changes from a feature branch into the main branch (such as the master branch) before merging them. Rebase works by moving or replaying the commits of one branch onto another.

When you perform a rebase, Git identifies the common ancestor commit of the two branches involved, then replays each commit from the feature branch on top of the destination branch, one by one. This process essentially makes it appear as if the commits from the feature branch were made directly on top of the destination branch. It results in a linear history without merge commits.


# Git Squash:
  Git squash is a technique used to combine multiple commits into a single commit. When you squash commits, Git collapses several commits into one, combining their changes into a single, coherent commit. This can help in creating a cleaner, more concise history with fewer commits.

To squash commits, you typically use an interactive rebase. During the rebase, you can specify which commits you want to squash together. Git will then combine the changes from those commits into one new commit. Squashing commits can be useful for cleaning up a branch's history before merging it into the main branch or creating more meaningful commits.

# Difference between Git Merge and Git Rebase:

  The main difference between git merge and git rebase lies in how they integrate changes from one branch into another:

  # Git Merge: 
  The git merge command combines the changes from one branch into another branch. It creates a new "merge commit" that has two or more parent commits, preserving the commit history of both branches. Merge commits visually represent the integration of changes from multiple branches. They are useful for maintaining a clear record of the different branches' histories and preserving branch relationships.

  # Git Rebase: 
  The git rebase command, on the other hand, integrates changes by moving or replaying commits from one branch onto another. It effectively makes it appear as if the commits were made directly on top of the destination branch, resulting in a linear commit history. Rebase is often used to incorporate changes from a feature branch into the main branch before merging, providing a cleaner, more straightforward history. However, it modifies the commit history of the target branch and can cause conflicts if multiple people are working on the same branch.



