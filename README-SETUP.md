# 🛠️ GitHub Profile README Setup & Customization Guide

Welcome to your **Premium Animated GitHub Profile README**! This guide outlines step-by-step instructions on how to publish, configure, and customize your profile to ensure all badges, dynamic cards, SVG assets, and links work seamlessly on your GitHub profile.

---

## 📂 Project Structure

Ensure your GitHub profile repository has the following file layout:

```text
Daksh-Gupta/             <-- Special repo matching your exact GitHub username
├── assets/
│   ├── hero-banner.svg      <-- Custom animated SVG banner
│   └── animated-divider.svg <-- Custom animated SVG divider line
├── README.md                <-- Your primary GitHub profile README
└── README-SETUP.md          <-- Setup & customization documentation (this file)
```

---

## 🚀 Quick Setup Instructions

### Step 1: Create Your GitHub Special Profile Repository

1. Log into your GitHub account.
2. Click the **`+`** icon in the top-right corner and select **New repository**.
3. In the **Repository name** field, type your exact GitHub username (e.g., if your username is `dakshgupta`, name the repository `dakshgupta`).
4. GitHub will show a banner saying: *"✨ You found a secret! `[username]/[username]` is a special repository..."*
5. Set the repository visibility to **Public**.
6. Check **Add a README file** (or leave unchecked if uploading files via Git CLI).
7. Click **Create repository**.

---

### Step 2: Upload Files to the Repository

#### Option A: Using Git CLI (Recommended)

Run the following commands in your local directory (`c:\Users\Daksh\Desktop\Gitubp`):

```bash
# Initialize git in workspace directory if needed
git init

# Add remote repository URL (replace YOUR_GITHUB_USERNAME with your username)
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME.git

# Stage all files including assets/
git add .

# Commit changes
git commit -m "feat: setup premium animated profile README"

# Push to GitHub main branch
git branch -M main
git push -u origin main
```

#### Option B: Upload via GitHub Web Interface

1. Open your special repository `https://github.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME`.
2. Drag and drop the `assets/` folder, `README.md`, and `README-SETUP.md` directly into the repository view.
3. Commit the files to `main`.

---

## ✏️ Step 3: Replace Placeholders in `README.md`

Open `README.md` in VS Code or your preferred text editor. Perform a **Find & Replace** (`Ctrl + H`) for the following placeholders:

| Placeholder String | What to Replace With | Example |
| :--- | :--- | :--- |
| `YOUR_GITHUB_USERNAME` | Your actual GitHub username | `dakshgupta` |
| `YOUR_LINKEDIN_USERNAME` | Your LinkedIn handle | `daksh-gupta` |
| `YOUR_LEETCODE_USERNAME` | Your LeetCode handle | `dakshgupta` |
| `YOUR-PORTFOLIO-URL.com` | Your personal portfolio domain | `dakshgupta.dev` |
| `your.email@example.com` | Your professional contact email | `daksh.gupta@example.com` |

---

## ⚡ Step 4: Customizing Specific Sections

### 1. Hero Animated Banner & Typing Effect
* The top banner points to `./assets/hero-banner.svg`. As long as the `assets/` folder is pushed to your repo root, GitHub will automatically render the vector graphic with animated glowing elements.
* To modify the typing animation titles, edit the `lines=` query parameter in the `readme-typing-svg` URL in `README.md`:
  ```html
  lines=Software+Engineer;Full-Stack+Developer;Backend+Enthusiast;DSA+Problem+Solver
  ```

### 2. Social Badges
Update the URLs inside the `<a>` tags surrounding each badge image:
```html
<a href="https://linkedin.com/in/YOUR_LINKEDIN_USERNAME">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
```

### 3. Dynamic GitHub Analytics & Streak Cards
The analytics cards automatically fetch live GitHub data using your username:
* **GitHub Stats:** `https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME...`
* **Streak Counter:** `https://github-readme-streak-stats.herokuapp.com/?user=YOUR_GITHUB_USERNAME...`
* **Top Languages:** `https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_GITHUB_USERNAME...`

> 💡 **Tip:** Make sure your GitHub contribution settings are set to show private contributions if you want your total streak and commits from private repositories to be counted! (GitHub Profile Settings -> Contribution Settings -> Private Contributions).

### 4. Featured Projects Section
The projects are organized inside clean GitHub-compatible HTML tables. Update the title, description, tech stack badges, and repository/live demo URLs for each project:
* **FitTrack AI**: Update `FitTrack` links to your actual repository.
* **FinPlan**: Update `FinPlan` links to your actual repository.
* **DevConnect**: Update `DevConnect` links.
* **AlgoViz**: Update `AlgoViz` links.

### 5. Problem Solving & LeetCode Integration
Replace `YOUR_LEETCODE_USERNAME` in the LeetCode card endpoints. The cards display your real-time LeetCode problem solving breakdown:
* `https://github-readme-leetcode.vercel.app/api?username=YOUR_LEETCODE_USERNAME&theme=dark`
* `https://leetcode-stats-api.herokuapp.com/YOUR_LEETCODE_USERNAME`

---

## 🔄 Step 5: Updating Your Profile Later

Whenever you want to update your profile (e.g. adding new projects, updating achievements, or tweaking tech stack icons):

1. Edit `README.md` locally.
2. Commit and push changes:
   ```bash
   git add README.md
   git commit -m "docs: update featured projects and tech stack"
   git push origin main
   ```
3. GitHub automatically updates your profile page immediately upon push!

---

## 🎨 Visual Assets Summary

* `assets/hero-banner.svg`: Sleek, dark developer header card with simulated IDE top-bar, animated circuit nodes, gradient typography, and glowing system badges.
* `assets/animated-divider.svg`: Lightweight glowing horizontal divider line with sliding accent light bead.

---

## ✅ Final Verification Checklist

Before publishing, double check:
- [ ] Special repo named exactly `<username>/<username>` created and set to **Public**.
- [ ] `assets/` folder uploaded containing both SVG files.
- [ ] Replaced all instances of `YOUR_GITHUB_USERNAME`.
- [ ] Replaced all social handle placeholders (`YOUR_LINKEDIN_USERNAME`, `YOUR_LEETCODE_USERNAME`, email, portfolio).
- [ ] Verified project links point to your actual GitHub repositories.
- [ ] Verified profile renders cleanly on both desktop and GitHub mobile app.

---

*Enjoy your state-of-the-art GitHub profile README!*
