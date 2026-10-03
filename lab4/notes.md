Question 1: What did --global mean here? What would happen if you left it out? Guess, then check with man git-config or ask.
ans- global tells to apply the recent configuration to all repositories for its current user on the current working computer .
Without --global, Git sets the configuration only for the current repository.
Question 2:What appeared in ls -a but not in ls? What is inside it?
ans- ls -a shows all the files including the hidden ones wheres ls shows only those files that the system wants to show.
.git contains Git's internal repository data, such as:

Commit history
Branch information
References to commits
Configuration
Staging/index information
Objects containing Git's stored versions of your files
Information needed to manage merges and conflicts
Question 3:Roughly how many files and folders is Git offering to track? Does anything in that list look like something you did not write?
ans: 6 , yes , .venv folder
Question 4:Compare this git status with the one from Question 3. What disappeared?
ans : .venv does not show up now.
Question 5
.gitignore itself shows up as untracked. Should it be committed, or ignored too? Why?
Yes, .gitignore should normally be committed to Git. ✅

.gitignore is not supposed to ignore itself. Its purpose is to tell Git which other files and folders should not be tracked.Why commit .gitignore?

Because .gitignore is part of the project's configuration..gitignore → should usually be tracked/committed.

The files listed inside .gitignore → should generally not be tracked.

Question 6
README.md moved from one heading to another in the git status output. Which two? In the three-places model from the session, what just happened to it?
ans:README.md now comes under : CHANGES TO BE COMMITTED ,it moved to this heading but initially it was under : UNTRACKED FILES. So it has been added to the staging place.
Question 7
What did Git print after the commit? How many files did it say changed?
ans:[master (root-commit) 9485ee2] Lab work so far
5 files changed, 218 insertions(+)
create mode 100644 .gitignore
create mode 100644  README.md 
create mode 100644  week02/dev tools.pdf
create mode 100644  week02/lab-log.txt
it changed 5 files
Question 8
What are the first seven characters of your commit called, and what are they for?
ans:The first seven characters are called the short commit hash (or short SHA).Git gives every commit a unique identifier called a commit hash.The full hash is much longer, but Git commonly displays the first 7 characters as a convenient short version.It lets you identify a specific commit.
Question 9
You now have two commits. Without looking it up: what are the four steps of the loop you just did twice?
ans:Change → Stage → Commit → Push
Question 10
Why does this file get a special name and a special place, rather than being called notes.md like everything else?
ans:Because it does not come under a folder unlike notes.md .
Question 11
What did gh auth login do that means you will not be asked for a password when you push?
ans:gh auth login authenticated your GitHub account and stored a credential/token securely on your computer.
GitHub can recognize that you are already authenticated, so you don't have to enter your GitHub password each time.
 Question 12
Refresh the repository page on GitHub. What is showing on the front page, and why that file?
ans:On the GitHub repository’s front page, we should see README.md (along with  other committed files).

Why README.md?
Because GitHub automatically uses a file named README.md as the repository’s main introduction/documentation. It displays its contents directly on the repository’s front page so visitors can immediately understand what the project is about.
So the key idea is:

README.md → GitHub recognizes it → displays it on the repository homepage.
Question 13
Run git log --oneline again. Did pushing change your local history in any way?
ans:No. Pushing did not change your local Git history.
you should see the same two commits as before.

Why?

git commit creates a commit in your local history.
git push copies your existing commits to GitHub.
It does not create a new commit or modify the local commits.
So:
Commit → changes local history
Push → uploads that history to GitHub
Question 14
Your repository is private but your TAs can now read it. In your own words, what is the difference between a repository being private and a repository not existing on GitHub at all?
ans:Being private means only the people whom we want to give access can see ou work and a repository not existing on GITHUB at all means it has not been created yet whether it is public or private nobody would be able to see the repository.