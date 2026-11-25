# Mission 2 — Become comfortable with the Terminal

## 1. Mission title

Mission 2 — Become comfortable with the Terminal

## 2. Task / objective

Use the command-line interface to inspect folders, create and manage practice files, understand flags and pipes, and explain package managers.

## 3. Work completed

### Task 2.1 — Basic Terminal operations

| Operation or command | What it does | What was observed |
|---|---|---|
| `pwd` | Displays the full absolute path of the current folder | The project folder was the current location |
| `ls` | Lists visible files and folders | The README, evidence, mission folders and practice folder were listed |
| `ls -la` | Uses detailed listing with hidden entries included | It showed file permissions, owner type, size, time and hidden entries such as `.` and `..` |
| `cd ..` | Moves to the parent folder | The location changed from the project folder to its parent |
| `mkdir` | Creates a new folder | `terminal-practice` was created inside the repository |
| `touch` | Creates an empty file when the file does not already exist | `practice.txt` and the first copy were created |
| `cp` | Copies a file to another name | `practice.txt` was copied before it was renamed |
| `mv` | Moves or renames a file | The copied file became `backup-copy.txt`, and later the backup became `practice-backup.txt` |
| `cat` | Displays a text file's contents | Both practice lines were visible |

### Task 2.2 — Safe file changes

The practice folder is `terminal-practice/`. It contains `practice.txt`, `practice-backup.txt`, and `backup-copy.txt`. The original file contains:

```text
First line
Second line
```

- Replacing a file's contents changes or erases the existing text, while appending adds text to the end and keeps earlier text.
- Copying creates a second file while leaving the original, but moving changes the file's location or name and does not leave it at the original location.
- `pwd` provides the absolute location of the current directory.
- Directory listing helps identify files, folders, hidden entries and their details.

### Task 2.3 — Flags and pipes

The normal `ls` listing showed visible names. `ls -la` showed hidden entries and detailed metadata. `ls -lah` additionally made sizes easier to read as bytes or kilobytes.

The command `ls -la | head -n 5` sent the detailed listing through the pipe `|` to `head`. `ls -la` produced the input, and `head -n 5` kept only the first five lines. Private usernames and full paths were not included in the Mission README or evidence.

### Task 2.4 — Package managers

Homebrew is installed, and `brew --version` reported version `7.0.7`. `brew list` showed installed packages such as Git and utility dependencies. A package manager helps install, update and remove software consistently, while tracking the packages managed for an environment. No packages were installed or removed.

## 4. Commands / tools used

- `pwd` — shows the current directory.
- `ls`, `ls -la`, `ls -lah` — display directory entries and options.
- `cd` — changes directories.
- `mkdir` — creates folders.
- `touch` — creates empty files.
- `cp` — copies files.
- `mv` — renames or moves files.
- `cat` — displays text files.
- `printf` and `>>` — add practice text to files.
- `head` and `|` — limit and pipe command output.
- `brew --version` and `brew list` — inspect Homebrew and managed packages without making changes.

## 5. My understanding

The Terminal allows file and directory operations to be performed precisely. Flags change command behavior, while pipes connect commands so output becomes input for the next command. Package managers make software management easier and more consistent.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- `terminal-practice/practice.txt`
- `terminal-practice/practice-backup.txt`
- `evidence/mission-02-terminal.txt`

## 9. Commit details

- Commit message: `Complete Terminal and file management mission`
- Status: Committed and pushed successfully to `main`.
