# Mission 6 — Git and GitHub

## 1. Mission title

Mission 6 — Git and GitHub

## 2. Task / objective

Understand version control, stage and commit changes, create a branch, open a Pull Request and explain the collaboration workflow.

## 3. Work completed

### Task 6.1 — Basic Git workflow

| Git operation | What it does |
|---|---|
| Check repository status | `git status` shows the branch, changed files and whether changes are staged |
| Stage selected changes | `git add` places selected file changes in the staging area for the next commit |
| Create a commit | `git commit` saves a snapshot of staged changes in the local repository |
| View commit history | `git log` shows recent commit messages, IDs and other history details |

Staging is the preparation step: selected changes are placed in the staging area. Committing then records those staged changes as a permanent snapshot with a message. A commit is still local until it is pushed to a remote repository.

### Task 6.2 — Branch

Created and switched to the branch `update-about`. Added a `## My Learning` section to the root `README.md`. After checking status and staging the README, committed the learning section and published the branch to GitHub.

### Task 6.3 — Pull Request

A branch is an independent line of development based on a commit. It lets work happen without changing the main line until it is reviewed.

A Pull Request proposes merging one branch into another and provides a place to review the changed files and discussion. It is useful because people can inspect work, identify problems and agree on changes before they become part of the shared branch.

The Pull Request and branch activity are visible on GitHub. It has not been merged unless the instructor explicitly requested merging.

### Task 6.4 — Git command glossary

| Operation | Meaning |
|---|---|
| Initialise a repository | `git init` creates a local Git repository and starts tracking history |
| Check status | `git status` reports branch and file-change state |
| Stage changes | `git add` puts selected changes into the next commit |
| Commit changes | `git commit` records staged changes in repository history |
| View history | `git log` displays commit history |
| Create or list branches | `git branch <name>` creates a branch; `git branch` lists branches |
| Switch branches | `git switch <branch>` changes the active working branch |
| Publish changes | `git push` sends local commits to a remote branch |
| Retrieve remote changes | `git pull` fetches and integrates remote changes |

## 4. Commands / tools used

- `git status` — inspected repository state.
- `git add` — staged selected changes.
- `git commit` — committed branch changes.
- `git log` — inspected recent history.
- `git switch -c update-about` — created and switched branches.
- `git push -u origin update-about` — published the branch.
- GitHub Pull Request — reviewed and proposed merging the README change.

## 5. My understanding

Git separates local work into branches and commits. The staging area lets me choose exactly what belongs in a commit. Branches and Pull Requests help isolate, review and combine work safely.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- Updated root `README.md` with My Learning
- `update-about` branch
- GitHub Pull Request

## 9. Commit details

- Pull Request: https://github.com/sky9977/digital-detective-8023/pull/1
- Pull Request status: Open; not merged because no instructor merge instruction was provided.
- Commit messages: `Add My Learning to root README`, `Document Mission 6 GitHub workflow`, and `Record Pull Request status`
- Status: Committed and pushed successfully.
