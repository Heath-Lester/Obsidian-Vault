<iframe width="100%" src="https://www.youtube-nocookie.com/embed/hwP7WQkmECE?si=XdmB41w-3tugHeK7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 4px; aspect-ratio: 16/9;"></iframe>

Git is a version control software that is used to track changes across a set of files.
- Initialize a repository with git by using `git init` in a terminal
- A commit is a snapshot of changes in a file
- Every commit is linked to a parent chain creating a timeline
- The head is the most recent commit, the head moves forward as you commit
- Simultaneous development is enabled through branching
- When branches are merged, all commits are merged together into a single timeline when they happened
- Conflicts occur when a merge is attempted but the parent history has changed where the code from your branch  has also changed
- Rebasing is when you re-write the history of your branch to a copy of another branch and then repositions all of your commits to the end.