# Linux
- Linux is a powerful, open source, UNIX-like operating system widely used in embedded systems, servers and general desktop usage.
- Extremely customisable for system administration and UI as well for eye candy.
- Highly flexible and secure. 
- A favourite among devs, sys admins and tech enthus.
- Linux is not a OS, but a kernel on top of which tech (like init system, core utils, user-space env, DEs and much more) is added to make it a full fledged OS.

---

# A Brief History
- 1991: Linux was created by Linus Torvalds, a Finnish computer science student, as a personal project to build a free, Unix-like kernel for his personal usage and then proceeded to publicly launch it once it came to a stable state.
- Open Source Growth: Released under the GNU General Public License (GPL), Linux quickly gained a global community of contributors who improved its kernel and tools.
- Linux Today: Now, Linux powers everything from web servers, supercomputers, and cloud platforms to smartphones (Android) and embedded devices.

---

# Linux Working
- **Kernel** - Core heart of the Operating systems that manages memory, processes and hardware peripherals
- **Shell** - Interact with the OS. Ex: Bash, Zsh, Fish.
- **File system and utils** - Programs, libs and tools to make the system usable.
---

## 1. Linux File System Structure

Linux uses a hierarchical file system. Key directories include:

| Directory | Description |
|-----------|-------------|
| `/`       | Root (top-level) directory |
| `/home`  | User home directories |
| `/etc`   | System configuration files |
| `/bin` / `/sbin` | Essential system binaries |
| `/usr`   | User utilities and applications |
| `/var`   | Variable data (logs, temp files) |
| `/tmp`   | Temporary files |

---

## 2. Essential Linux Commands

### Navigation and File Management

| Command | Description | Example / Notes |
|---------|-------------|----------------|
| `pwd`   | Print working directory | |
| `ls`    | List files and directories | `ls -l` (long), `ls -a` (show hidden) |
| `cd`    | Change directory | `cd ..` (up), `cd ~` (home) |
| `mkdir` | Create a new directory | `mkdir newDir` |
| `touch` | Create empty file or update timestamps | `touch file.txt` |
| `cp`    | Copy files or directories | `cp file1 file2` |
| `mv`    | Move or rename files | `mv old.txt new.txt` |
| `rm`    | Remove files or directories | `rm file.txt`, `rm -r folder` |


### Viewing File Contents

| Command | Description | Example / Notes |
|---------|-------------|----------------|
| `cat`   | Display entire file content | |
| `head`  | Show beginning of a file | `head -n 10 file.txt` |
| `tail`  | Show end of a file | `tail -n 10 file.txt` |
| `less`  | View file page by page | Navigate with arrow keys, q to quit |

### File Permissions

| Command | Description | Example |
|---------|-------------|---------|
| `chmod` | Change file permissions | `chmod 777 file.txt` |
| `chown` | Change file owner | `chown user:group file.txt` |
| `ls -l` | View file permissions | |

### Searching and Filtering

| Command | Description | Example |
|---------|-------------|---------|
| `grep`  | Search for patterns in files | `grep "password" file.txt` |
| `find`  | Search for files/directories | `find . -name "flag.txt"` |
| `awk`   | Pattern scanning and processing | `awk '{print $1}' file.txt` |
| `sed`   | Stream editor for text | `sed 's/old/new/' file.txt` |

### File Analysis & CTF Tools

| Command | Description | Example / Notes |
|---------|-------------|----------------|
| `file`  | Determine file type | `file binary` |
| `strings` | Extract readable text from binaries | `strings binary` |
| `hexdump` | Hex dump alternative | `hexdump -C file` |
| `tar`   | Extract tar archives | `tar -xvf file.tar` |
| `gunzip` | Unzip .gz files | `gunzip file.gz` |


---

# Misc
- If you want to know about all the flags or more detailed version of your ctf, then use the `man` command. Ex: `man ls`

---

## 3. CTF Tips

- Inspect file permissions and look for hidden files—they often hide the clues.  
- Run `strings` on binary files to reveal any human-readable information.  
-Chain commands using pipes (`|`) to filter and process data efficiently.
    - For example: `strings <file> | grep "text"`
- Experiment and practice frequently—real mastery comes from doing.

---

## 4. Practice picoCTF Challenges

- [picoCTF 301](https://play.picoctf.org/practice/challenge/301)  
- [picoCTF 300](https://play.picoctf.org/practice/challenge/300)  
- [picoCTF 137](https://play.picoctf.org/practice/challenge/137)  
- [picoCTF 285](https://play.picoctf.org/practice/challenge/285)  

---

# Linux Cheatsheet
- [Linux Command Line](https://cheatography.com/davechild/cheat-sheets/linux-command-line/)
- [Shell Scripting](https://www.shellscript.sh)
