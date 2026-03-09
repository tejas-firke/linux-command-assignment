# 🐧 Linux Commands Assignment — AWS EC2

> **Author:** Tejas Firke  
> **Platform:** AWS EC2 (Ubuntu)  
> **Objective:** Practice and document essential Linux commands with screenshots

---

## 📋 Overview

This assignment covers hands-on practice of fundamental Linux commands executed on an **AWS EC2 instance**. Each section includes the command used, a clear explanation of what it does, and a screenshot for reference.

---

## 📁 Repository Structure

```
linux-commands-assignment/
│
├── README.md                        # This file
├── linux_commands_assignment.docx   # Original assignment document
│
└── screenshots/
    ├── 01_creating_renaming.png     # mkdir, cd, touch, mv
    ├── 02_viewing_file_contents.png # cat, head, tail
    ├── 03_searching_patterns.png    # grep
    ├── 04_zipping_unzipping.png     # zip, unzip
    ├── 05_downloading_files.png     # wget
    ├── 06_changing_permissions.png  # chmod, ls -l
    └── 07_environment_variables.png # export, echo
```

---

## 🗂️ Topics Covered

### 1. 📂 Creating and Renaming Files/Directories
| Command | Description |
|--------|-------------|
| `mkdir test_dir` | Creates a new directory named `test_dir` |
| `cd test_dir` | Changes current directory to `test_dir` |
| `touch example.txt` | Creates an empty file named `example.txt` |
| `mv example.txt renamed_example.txt` | Renames `example.txt` to `renamed_example.txt` |

---

### 2. 👁️ Viewing File Contents
| Command | Description |
|--------|-------------|
| `cat /etc/passwd` | Displays the full content of `/etc/passwd` |
| `head -n 5 /etc/passwd` | Displays the **first** 5 lines of the file |
| `tail -n 5 /etc/passwd` | Displays the **last** 5 lines of the file |

---

### 3. 🔍 Searching for Patterns
| Command | Description |
|--------|-------------|
| `grep root /etc/passwd` | Searches for lines containing `root` in `/etc/passwd` |

---

### 4. 🗜️ Zipping and Unzipping
| Command | Description |
|--------|-------------|
| `zip -r test_dir.zip test_dir` | Compresses `test_dir` into `test_dir.zip` |
| `mkdir unzipped_dir` | Creates a new directory `unzipped_dir` |
| `unzip test_dir.zip -d unzipped_dir` | Extracts zip contents into `unzipped_dir` |

---

### 5. 🌐 Downloading Files
| Command | Description |
|--------|-------------|
| `wget https://example.com/sample.txt` | Downloads a file from the internet into the current directory |

---

### 6. 🔐 Changing Permissions
| Command | Description |
|--------|-------------|
| `touch secure.txt` | Creates a file named `secure.txt` |
| `chmod 444 secure.txt` | Sets file to **read-only** for all users |
| `ls -l secure.txt` | Displays file permissions |

---

### 7. 🌿 Working with Environment Variables
| Command | Description |
|--------|-------------|
| `export MY_VAR='Hello, Linux!'` | Creates a new environment variable `MY_VAR` |
| `echo $MY_VAR` | Displays the value of the environment variable |

---

## 🛠️ Setup

These commands were executed on an **AWS EC2 Ubuntu instance**. To replicate:

1. Launch an EC2 instance (Ubuntu 22.04 recommended)
2. Connect via SSH:
   ```bash
   ssh -i your-key.pem ubuntu@your-ec2-ip
   ```
3. Run the commands from each section above

---

