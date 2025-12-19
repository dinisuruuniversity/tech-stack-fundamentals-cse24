# Tech Stack Fundamentals Workshops

---

## Repository Structure

```
tech-stack-fundamentals-cse24/
├── README.md
├── WORKSHOP_OVERVIEW.md
├── SCHEDULE.md
├── Task 01/
│   ├── README.md
│   ├── task_instructions.pdf
│   └── submissions/
│       └── [Your_Name]/
│           ├── index.html
│           ├── style.css
│           └── images/
├── Task 02/
│   ├── README.md
│   ├── task_instructions.pdf
│   └── submissions/
│       └── [Your_Name]/
│           └── index.html
└── Task 03/
    ├── README.md
    ├── task_instructions.pdf
    └── submissions/
        └── [Your_Name]/
            └── index.html
```

---

## How to Submit Your Work

> ⚠️ **Important:** You cannot push directly to this repository. All submissions must be made through **Pull Requests**.

### Step 1: Fork the Repository

1. Go to [https://github.com/HimathX/tech-stack-fundamentals-cse24](https://github.com/HimathX/tech-stack-fundamentals-cse24)
2. Click the **"Fork"** button (top-right corner)
3. This creates a copy of the repository under your GitHub account

### Step 2: Clone Your Forked Repository

```bash
git clone https://github.com/YOUR_USERNAME/tech-stack-fundamentals-cse24.git
cd tech-stack-fundamentals-cse24
```

> Replace `YOUR_USERNAME` with your GitHub username

### Step 3: Create Your Submission Folder

**Naming Format:** `[First_Name]_[Last_Name]`

```bash
# Navigate to task submissions folder
cd "Task 01/submissions"

# Create your folder
mkdir Himath_Jayasinghe
cd Himath_Jayasinghe

# Create your HTML file
code index.html
```

**Examples:**
- `Himath_Jayasinghe/index.html`
- `Anusha_Perera/index.html`
- `Kamal_Silva/index.html`

### Step 4: Complete Your Task

Write your code in `index.html` according to the task instructions in the README.md of that task folder.

### Step 5: Commit and Push to Your Fork

```bash
# Return to repository root
cd ../../..

# Stage your changes
git add .

# Commit with clear message
git commit -m "Add Task 1: Himath Jayasinghe"

# Push to YOUR forked repository
git push origin main
```

### Step 6: Create a Pull Request

1. Go to your forked repository on GitHub
2. Click the **"Contribute"** button → **"Open pull request"**
3. Or click the **"Compare & pull request"** button if it appears
4. Add a clear title: `Task 1 Submission: Your Name`
5. Add a description of your work (optional)
6. Click **"Create pull request"**
7. Wait for your submission to be reviewed and merged! ✅

---

## Keeping Your Fork Updated

Before starting a new task, sync your fork with the original repository:

```bash
# Add the original repository as upstream (only needed once)
git remote add upstream https://github.com/HimathX/tech-stack-fundamentals-cse24.git

# Fetch and merge updates
git fetch upstream
git merge upstream/main

# Push updates to your fork
git push origin main
```

---

## Quick Reference

```bash
# 1. Fork the repository on GitHub first!

# 2. Clone YOUR fork
git clone https://github.com/YOUR_USERNAME/tech-stack-fundamentals-cse24.git

# 3. Create submission folder
cd "Task 01/submissions"
mkdir Your_Name
cd Your_Name

# 4. Create index.html
code index.html

# 5. Stage and commit
cd ../../..
git add .
git commit -m "Task 1: Your Name"
git push origin main

# 6. Go to GitHub and create a Pull Request!
```

---

## Troubleshooting

**Cannot push to repository?**

You're likely trying to push to the original repository instead of your fork. Make sure you cloned YOUR fork:
```bash
# Check your remote URL
git remote -v

# It should show YOUR username, not HimathX
# If wrong, update it:
git remote set-url origin https://github.com/YOUR_USERNAME/tech-stack-fundamentals-cse24.git
```

**Pull Request has conflicts?**

Sync your fork with the original repository:
```bash
git fetch upstream
git merge upstream/main
# Resolve any conflicts
git add .
git commit -m "Resolve merge conflicts"
git push origin main
```

**Forgot to fork first?**
1. Fork the repository on GitHub
2. Update your remote URL:
```bash
git remote set-url origin https://github.com/YOUR_USERNAME/tech-stack-fundamentals-cse24.git
git push origin main
```

---

## 🖥️ Using GitHub Desktop (Alternative Method)

If you prefer a graphical interface instead of command line:

### Step 1: Install GitHub Desktop

Download from [https://desktop.github.com/](https://desktop.github.com/) and sign in with your GitHub account.

### Step 2: Fork the Repository

1. Go to [https://github.com/HimathX/tech-stack-fundamentals-cse24](https://github.com/HimathX/tech-stack-fundamentals-cse24)
2. Click the **"Fork"** button (top-right corner)

### Step 3: Clone Your Fork in GitHub Desktop

1. Open GitHub Desktop
2. Go to **File** → **Clone Repository**
3. Select the **GitHub.com** tab
4. Find `tech-stack-fundamentals-cse24` in your repositories list
5. Choose where to save it on your computer
6. Click **Clone**

### Step 4: Create Your Submission

1. Open the repository folder in File Explorer
2. Navigate to `Task 01/submissions/`
3. Create a new folder with your name (e.g., `Himath_Jayasinghe`)
4. Add your files: `index.html`, `style.css`, and `images/` folder

### Step 5: Commit Your Changes

1. Open GitHub Desktop - it will show your changes
2. In the bottom-left, add a **Summary**: `Task 1 Submission: Your Name`
3. Click **Commit to main**

### Step 6: Push to GitHub

1. Click **Push origin** (or **Publish branch**)

### Step 7: Create a Pull Request

1. In GitHub Desktop, go to **Branch** → **Create Pull Request**
2. This opens GitHub in your browser
3. Add a title: `Task 1 Submission: Your Name`
4. Click **Create pull request**
5. Done! Wait for your submission to be reviewed ✅

### Keeping Your Fork Updated (GitHub Desktop)

1. In GitHub Desktop, go to **Branch** → **Merge into current branch**
2. Select **upstream/main**
3. Click **Merge upstream/main into main**
4. Click **Push origin**

> 💡 **Tip:** If you don't see upstream, go to **Repository** → **Repository settings** → **Remote** and add the original repo URL.

---

Last Updated: 19th December 2025
