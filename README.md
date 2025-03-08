Git Version Control & Collaboration Assignment Documentation

Task 1: Version Control & Branching
Step 1: Creating a New Repository
To start, I collaborated with a team member to complete this assignment. We first created a new repository on GitHub.

1. Logged in to GitHub (or any Git hosting service).
2. Clicked on **New Repository**.
3. Entered a repository name and description.
4. Initialized with a README file (optional) and clicked **Create Repository**.

 Step 2: Cloning the Repository

git clone https://github.com/<my-username>/<repository-name>.git
cd <repository-name>
```

Step 3: Creating a Feature Branch
```bash
git checkout -b feature-update
```

### **Step 4: Adding a README.md File**
I added a `README.md` file with a short introduction about myself.
```bash
echo "# About Me" > README.md
```

### **Step 5: Committing & Pushing Changes**
```bash
git add README.md
git commit -m "Added README.md with personal introduction"
git push origin feature-update
```

### **Step 6: Opening a Pull Request (PR)**
1. Went to the repository on GitHub.
2. Clicked **Compare & pull request**.
3. Added a description and clicked **Create pull request**.

### **Step 7: Reviewing & Merging PR**
- Reviewed the changes with my collaborator.
- Clicked **Merge pull request**.

---

## **Task 2: Team Collaboration (Pair Programming)**
### **Step 1: Repository Creation & Invitation**
I worked with a group member on this task. One of us created a repository and invited the other as a collaborator. The repository owner added an `index.html` file and pushed it to `main`.

### **Step 2: Cloning & Creating a New Branch**
As the collaborator, I cloned the repo:
```bash
git clone https://github.com/<owner-username>/<repository-name>.git
cd <repository-name>
git checkout -b update-styles
```

### **Step 3: Modifying index.html & Pushing Changes**
I modified `index.html` by adding a `<style>` section.
```bash
git add index.html
git commit -m "Added basic styles to index.html"
git push origin update-styles
```

### **Step 4: Creating & Merging a PR**
- I opened a PR.
- My collaborator reviewed and merged it.
- We both pulled the latest changes to stay updated.

```bash
git pull origin main
```

---

## **Task 3: Resolving Merge Conflicts**
### **Step 1: Creating & Editing a Branch**
Each of us created our own repository and attempted to create a merge conflict intentionally.

1. Cloned the repository.
2. Created a new branch and modified a file.
```bash
git checkout -b edit-text
echo "New content" >> file.txt
git commit -am "Edited file.txt"
```

### **Step 2: Creating a Conflict**
We switched to `main` and modified the same file differently.
```bash
git checkout main
echo "Conflicting content" >> file.txt
git commit -am "Updated file.txt in main"
```

### **Step 3: Merging & Resolving Conflicts**
```bash
git merge edit-text
```
After manually resolving the conflict, we committed the final version:
```bash
git add file.txt
git commit -m "Resolved merge conflict in file.txt"
git push origin main
```

---

## **Task 4: Working with a Remote Repository**
### **Step 1: Forking & Cloning a Repository**
As part of the assignment, we forked an open-source project on GitHub and cloned it locally.
```bash
git clone https://github.com/<my-username>/<repository-name>.git
```

### **Step 2: Creating a Documentation Branch**
```bash
git checkout -b documentation-update
```

### **Step 3: Updating Documentation**
We worked together to edit `README.md` and `CONTRIBUTING.md` by adding an installation guide and improving formatting.
```md
## Installation Guide
Run:
```bash
npm install
```
```

### **Step 4: Committing & Pushing Changes**
```bash
git add .
git commit -m "Updated documentation"
git push origin documentation-update
```

### **Step 5: Creating a PR & Receiving Feedback**
- We opened a PR and waited for feedback from the project maintainers.
- Based on feedback, we made necessary changes.
- Once approved, the PR was merged.

### **Step 6: Syncing the Fork**
```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

## **Conclusion**
Through collaboration, we successfully completed the assignment, gaining hands-on experience with:
- Creating and managing branches
- Working with pull requests
- Resolving merge conflicts
- Contributing to open-source projects

This experience reinforced best practices in Git and GitHub while improving our teamwork and problem-solving skills.



