# How to create a repo for first time in GitHub

### Create a new directory
```bash
mkdir test-repo
cd test-repo
```

### Initialize Git

```bash
git init
```

### Create a file

```bash
echo "# Test Repository" > README.md
```

### Stage and commit

```bash
git add README.md
git commit -m "Initial commit"
```

### Create Gihub repo and push

```bash
gh repo create test-repo —public —source=. —push 
```

### This gh repo create command does three things at once:
### 1. Creates a new public repository on GitHub named test-repo.
### 2. Links your local repository to it (by setting the origin remote).
### 3. Pushes your "Initial commit" to the main branch on GitHub.

---
### Using Manual Git Commands
### The repo must be created on the website
### Create a repository on GitHub, then:
### (Assuming you've already done mkdir, cd, git init, git add, git commit)

```bash
git remote add origin https://github.com/YourUsername/test-repo.git
```

# Now you can push

```bash
git push -u origin main
```