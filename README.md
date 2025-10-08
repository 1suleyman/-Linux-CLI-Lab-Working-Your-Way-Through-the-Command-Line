# 🐧 Linux CLI Lab – Working Your Way Through the Command Line

In this lab, I practiced essential **file and directory management** skills using Linux command line tools. The lab focuses on creating, moving, copying, and removing files and directories, as well as working with nested directory hierarchies.

---

## 📋 Lab Overview

**Goal:**

* Understand the Linux file system structure
* Learn to create, edit, and delete files and directories
* Practice navigating directories and manipulating file content
* Handle hierarchical directories using `mkdir -p`
* Move, copy, and remove files and directories safely

**Learning Outcomes:**

* Master CLI commands: `ls`, `touch`, `cat`, `mkdir`, `mv`, `rm`
* Understand file paths and nested directory structures
* Practice text redirection and file content management
* Gain confidence in safely manipulating the Linux filesystem

---

## 🛠 Step-by-Step Journey

### Step 1: Count directories and files

```bash
ls /home/four44/test_dir
# Result: 3 directories, 3 files
```

---

### Step 2: Identify missing file

* Missing file: `test_file3.txt`
* Verified by listing directory contents:

```bash
ls /home/four44/test_dir
```

---

### Step 3: Create an empty file

```bash
touch /home/thor/empty_file.txt
ls /home/thor
```

---

### Step 4: Create a file with content

```bash
cat > /home/thor/contents_file.txt
This is not an empty file
<Ctrl-D>
cat /home/thor/contents_file.txt
```

---

### Step 5: Create an empty directory

```bash
mkdir /home/thor/MT_DIR
```

---

### Step 6: Create a nested directory hierarchy

```bash
mkdir -p /home/thor/asia/india/bangalore
```

* `-p` ensures parent directories are created automatically.

---

### Step 7: Move a target file to a directory

```bash
mv /home/four44/asia/bangalore.txt /home/thor/asia/india/bangalore/
```

* Ensures the file is in the correct hierarchical location.

---

### Step 8: Copy a source directory to a target location

```bash
mv /home/thor/asia/india/bangalore /home/thor/
```

* Moved directory including its contents.

---

### Step 9: Remove a file from a directory

```bash
rm /home/thor/asia/bangalore.txt
```

* Checks if file exists; safe removal.

---

### Step 10: Remove a directory and its contents

```bash
rm -r /home/thor/asia/india/bangalore
```

* `-r` removes all files and subdirectories recursively.

---

## ✅ Key Commands Summary

| Task                      | Command / Notes                          |
| ------------------------- | ---------------------------------------- |
| List files/directories    | `ls /path/to/directory`                  |
| Create empty file         | `touch /path/to/file.txt`                |
| Create file with content  | `cat > /path/to/file.txt`                |
| Create empty directory    | `mkdir /path/to/directory`               |
| Create nested directories | `mkdir -p /path/to/nested/directory`     |
| Move file                 | `mv /source/file /target/directory/`     |
| Move directory            | `mv /source/directory /target/location/` |
| Remove file               | `rm /path/to/file`                       |
| Remove directory          | `rm -r /path/to/directory`               |

---

## 💡 Notes / Tips

* Use `mkdir -p` to create nested directories in one command.
* Use `cat > file.txt` and `<Ctrl-D>` to quickly add content to a file.
* Always double-check paths before `rm -r` to avoid accidental deletion.
* Moving files/directories overwrites content if a file with the same name exists.

---

## 📌 Lab Summary

| Step                      | Status | Key Takeaways                              |
| ------------------------- | ------ | ------------------------------------------ |
| Count files/directories   | ✅      | Verified number of directories and files   |
| Identify missing file     | ✅      | Found `test_file3.txt` missing             |
| Create empty file         | ✅      | Learned `touch` command                    |
| Create file with content  | ✅      | Learned text redirection with `cat > file` |
| Create empty directory    | ✅      | Learned `mkdir` command                    |
| Create nested directories | ✅      | Learned `mkdir -p` for hierarchy           |
| Move a file               | ✅      | Practiced moving files with `mv`           |
| Move a directory          | ✅      | Practiced moving directories               |
| Remove file               | ✅      | Learned `rm` command                       |
| Remove directory          | ✅      | Learned `rm -r` for recursive removal      |

