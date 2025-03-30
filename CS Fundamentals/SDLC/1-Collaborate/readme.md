## Git and Github 

A repository (repo) is a storage location where all the files, folders, and version history of a project are stored. It helps manage and track changes in software development.

Git is a version control cli tool, for pushing changes to a repository 

Github stores repositories on the cloud (GitHub servers). 

### How to setup Git and Github

Create a GitHub Account
Setup Git >>  https://www.geeksforgeeks.org/install-git-on-windows/
Add git to path during installation
openSSL to allow Git to communicate securely over HTTPS.
Check path variables in advanced system settings (user or system variables)
git –version

The full form of OpenSSH is OpenBSD Secure Shell. It's an open-source implementation of the Secure Shell (SSH) protocol, providing secure networking utilities for remote access and secure file transfer. 

Git commands 

```
git init            # Create a new local repository
git clone <URL>     # Copy a remote repository
git add .           # Stage all changes
git commit -m "msg" # Save changes with a message
git push            # Upload changes to a remote repository
git pull            # Get latest changes from a remote repository
git checkout -b learnHowToCode     # Create a separate branch on local and do all you experimentation there
```

### Difference between https and ssh cloning 

1️⃣ HTTPS Cloning
📌 Example Command:
git clone https://github.com/user/repo.git

✅ Pros:
✔️ Easier to use – No extra setup required.
✔️ Secure encryption using TLS (SSL).
❌ Cons:
❌ Requires entering a GitHub username and password every time (or a Personal Access Token for authentication).
 ❌ Slower than SSH due to extra authentication steps.

2️⃣ SSH Cloning
📌 Example Command:
git clone git@github.com:user/repo.git

✅ Pros:
✔️ More secure – Uses SSH key authentication instead of passwords.
 ✔️ No need to enter credentials every time (after setting up SSH keys).
 ✔️ Faster compared to HTTPS.
❌ Cons:
❌ Requires SSH key setup (ssh-keygen + adding the key to GitHub).

