# Linux Basics Lab – Day 2

## Objective

Practice file management, permissions, and command-line operations in a Linux environment for cybersecurity applications.

## Lab Environment

Operating System: Parrot OS
Platform: UTM (Mac M1)

---

## Commands Practiced

### File Creation & Viewing

* `touch filename` – Create a new file
* `cat filename` – Display file content
* `echo "text"` – Print text to terminal
* `echo "text" > file` – Overwrite file content
* `echo "text" >> file` – Append content to file

---

### File Editing

* `nano filename` – Edit file in terminal
* `pluma filename` – Open GUI text editor

---

### File & Directory Management

* `cp source destination` – Copy files
* `mv source destination` – Move or rename files
* `mkdir dirname` – Create directory
* `mkdir -p dir1/dir2/dir3` – Create nested directories
* `rm file` – Delete file
* `rm -r directory` – Delete directory recursively

---

### Navigation & Listing

* `ls` – List files
* `ls -l` – Detailed file listing
* `pwd` – Show current directory
* `tree` – Display directory structure

---

### File Information

* `file filename` – Identify file type

---

### Permissions & Execution

* `chmod u+x file` – Add execute permission to user

* `chmod g-r file` – Remove read permission from group

* `chmod o+r file` – Add read permission to others

* `chmod ugo+rwx file` – Full permissions to all

* `chmod ugo-rwx file` – Remove all permissions

* `./file` – Execute file

---

### Wildcards Usage

* `chmod o-rwx D*` – Apply to files starting with "D"
* `chmod g-rwx *s` – Apply to files ending with "s"
* `chmod g-rwx *` – Apply to all files

---

## Key Takeaways

* Learned how Linux handles file permissions using `chmod`
* Understood how to safely create, modify, and delete files
* Practiced command chaining and file redirection
* Gained hands-on experience with directory structures

---

## Cybersecurity Relevance

* File permissions are critical for **system security and access control**
* Command-line skills are essential for **penetration testing and SOC roles**
* Redirection (`>`, `>>`) is widely used in **logging and scripting**

---

## Next Steps

* Practice user and group management
* Learn networking commands (`ifconfig`, `ip a`, `ping`)
* Begin network scanning tools like Nmap
