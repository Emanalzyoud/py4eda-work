 HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.
### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`
# Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL: ...
- Output of `git remote -v`:
- The output of `git log --oneline`:



## Questions

### Reflections

#### Question 1: Git Workflow Benefits
**a)** Before this homework I mostly handled versions by saving new files or adding “final2” to the name, or just trusting whatever I last uploaded. It works, but it’s messy and I can’t tell what actually changed. With Git I get:
1. a timeline of changes with messages,
2. the ability to pick which files go in the commit,
3. and I can push it to GitHub so it’s backed up and public.

**b)** A situation where Git would’ve helped: I’ve edited something, then later realized I liked the earlier version better. If it was in Git, I could just look at the history and go back to that commit instead of trying to remember what I did.



#### Question 2: Repository Organization
**a)** The two repos are for two different purposes. The `class_repo` is the instructor’s — I only pull from it. My `my_repo` is the one I control and push to GitHub. If I tried to mix them, I could run into permission errors (because I can’t push to the class repo) and it would be harder to keep the instructor’s copy clean.

**b)** Going forward I’d keep the same idea: one repo that’s “my course work,” separate repos for group projects, and then any instructor/reference repo stays separate as a clone. That keeps ownership clear.



#### Question 3: Commit Messages and History
**a)** A commit like “update” doesn’t tell me anything later. “Add hw3a solution documenting Git workflow and repository structure” tells me what I actually did. That’s useful if I need to prove when I finished something or if I want to copy that text into another place.

**b)** On a longer project I’d commit in small, finished chunks — e.g. “data loaded,” “cleaning done,” “README updated,” “typo fixed.” If I can explain the change in one short sentence, it’s a good commit.



### Graduate Questions

#### Question 1: The Three-Stage Model
**a)** Doing the first commit with just `README.md` and `.gitignore` makes the start of the repo look clean — it’s the “setup” commit. Then adding the homework file as a second commit makes the history easier to read. If I dumped everything in one commit, setup and actual work would be mixed.

**b)** From that list:
- load data → commit (it’s a complete step),
- half-finished function → don’t commit yet,
- typo fix → ok to commit,
- README update → commit.
Staging lets me pick only the finished parts.

**c)** I should run `git status` a lot so I know what state I’m in — what’s untracked, what’s staged, what’s going to be committed.



#### Question 2: Local vs. Remote Repositories
**a)** “Distributed” just means every clone has the whole repo and its history, not just a link to GitHub. That’s different from Drive/Dropbox where you don’t have commits.

**b)** That’s nice because I can keep working and committing even if I’m offline, and then later do `git push` when I have internet.

**c)**  
- `git clone` → first download,  
- `git pull` → get updates from GitHub,  
- `git push` → send my updates to GitHub.  
I can’t push to `class_repo` because I don’t own it; I can push to `my_repo` because I do.



#### Question 3: Professional Portfolio
**a)** I should commit things that show progress, but not stuff that shouldn’t be public (big data files, secrets). It’s fine to show the steps as long as the main branch stays readable.

**b)** For this class repo, the README should say who I am, what the course is, and what’s inside. An open-source README is more about install/run instructions.

**c)** Doing this during the semester builds a real history instead of trying to make one when just need it . Good habits: meaningful commit messages, push often, keep the repo tidy.

