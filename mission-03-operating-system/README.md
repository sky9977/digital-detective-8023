# Mission 3 — Understand the operating system

## 1. Mission title

Mission 3 — Understand the operating system

## 2. Task / objective

Explore the operating system, running processes, storage, paths and file permissions, and describe operating-system responsibilities.

## 3. Work completed

### Task 3.1 — Explore your operating system

| Information explored | What it tells you | Privacy-safe observation |
|---|---|---|
| Operating system and system details | Identifies the operating-system environment and version | macOS 26.6.2 |
| Current account identity | Identifies the account used for the session | `[redacted]` |
| Available and used storage | Shows capacity, used space and available space | 460 GiB capacity; 15 GiB used and 95 GiB available at the observed time |
| System activity snapshot | Shows process count and current resource use | 626 total processes, 5 running and 621 sleeping; 61.44% user CPU, 11.30% system CPU and 27.24% idle CPU |

### Task 3.2 — Understand processes

A process is a program or system task that is currently running. The PID column, or process identifier, gives each process a unique identification number while it is active. Examples observed include `launchd`, the macOS system process manager, and `logd`, a system logging process.

### Task 3.3 — Understand paths and permissions

An absolute path gives the complete location from the file-system root. The absolute assignment path observed was `/Users/[redacted]/digital-detective-8023`. A relative path begins from the current folder. From the project folder, `mission-02-terminal` is a relative path to that mission folder.

The practice file `terminal-practice/practice.txt` had `-rw-r--r--` in the detailed listing. For the owner, `r` means read, `w` means write and `-` means execute is not granted. Therefore, the owner can read and change the file but cannot execute it as a program. The listing does not show that the file was changed.

| Permission | Meaning | Example |
|---|---|---|
| `r` — Read | Allows contents to be read | Opening a text file |
| `w` — Write | Allows contents to be changed | Editing a text file |
| `x` — Execute | Allows a program or script to run; for a directory, allows traversal | Running an executable script |

### Task 3.4 — Operating-system responsibilities

| OS responsibility | My explanation | Example |
|---|---|---|
| Process management | Starts, schedules and stops running programs | macOS lets Terminal and a text editor run at the same time |
| Memory management | Allocates memory to programs and recovers unused memory | RAM holds document text while it is being edited |
| Device management | Controls communication with hardware through drivers | The OS sends display information to the monitor |
| File management | Creates, finds, protects and organizes files and folders | The assignment folder stores README and mission files |
| User interface or shell | Provides a graphical interface or command-line way to communicate with the OS | Terminal accepts commands typed by the user |
| Security and permissions | Controls access to files and system resources | `rw-r--r--` lets the owner read and write, while other users only read |

## 4. Commands / tools used

- `sw_vers` — checked the macOS product name and version.
- `whoami` — identified the active account, then redacted in evidence.
- `df -h /` — checked storage capacity and usage.
- `top -l 1 -n 8` — captured a brief system activity snapshot.
- `ps -axo pid,comm` — viewed process IDs and process names.
- `pwd` — checked the current absolute location.
- `ls -l` and `ls -ld` — observed file and directory permissions.

## 5. My understanding

The operating system is the middle layer between hardware and applications. It manages processes, memory, devices, files and user permissions. Absolute paths describe a complete location, while relative paths depend on the current folder. PIDs help the system identify processes, and permission characters indicate allowed actions.

## 6. Difficulties faced

No major difficulties.

## 7. How I resolved them

Not applicable.

## 8. Evidence / files

- `evidence/mission-03-operating-system.txt`
- Privacy-safe process and system observations

## 9. Commit details

- Commit message: `Document operating system and file management`
- Status: Committed and pushed successfully to `main`.
