# 🚀 GitHub Setup Guide & Source Code Management (SCM) Overview

## 📌 What is GitHub?
GitHub is a **cloud-based platform** that provides **distributed version control** and **source code management (SCM)** using Git.  
It enables:
- Team collaboration on code.
- Issue tracking & project management.
- CI/CD automation using **GitHub Actions**.
- Secure code hosting for both public and private repositories.

---

## 💬 Popular Communication Tools
These tools are often used **alongside GitHub** for team collaboration:
- Microsoft Teams  
- Slack  
- Skype for Business  
- Discord  
- Google Chat  

---

## 🗂️ Source Code Management (SCM) Tools
Widely used SCM tools include:
- GitHub  
- Bitbucket  
- GitLab  
- SVN (Subversion)  
- TFS (Team Foundation Server)  
- CVS (Concurrent Versions System)  

---

## ⚙️ GitHub Administration Steps

### ✅ Step 1: Create a GitHub Account
- Use your **official/work email**  
- Choose a strong password & enable **2FA**  
- URLs:  
  - Public GitHub → [https://github.com/](https://github.com/)  
  - Enterprise GitHub → Example: `https://airtel.github.com/`  

---

### ✅ Step 2: Log in to GitHub
- Go to GitHub login page.  
- Enter credentials → Access dashboard.  

---

### ✅ Step 3: Create an Organization
- Example Organization: **bsnl-4g-test**  
- **Use service accounts only (not personal emails)**:
  - ❌ `kkeducationblr@gmail.com`  
  - ❌ `prasanth@bsnl.com`  
  - ✅ `devops4g@bsnl.com`  

---

### ✅ Step 4: Create Repositories
- 🔒 **Private Repo:** `testing-private-repo`  
- 🌐 **Public Repo:** `testing-public-repo`  
- Best Practices:
  - Use meaningful repo names.
  - Initialize with README.md & `.gitignore`.
  - Apply licenses (MIT, Apache, etc.) where applicable.

---

### ✅ Step 5: Create Teams
- **Dev Team** → `bsnl-dev-team`  
- **DevOps Team** → `bsnl-DevOps-Team`  
- (Optional) QA, SRE, DB Teams.  

---

### ✅ Step 6: Add Users to Teams
- Assign GitHub usernames or verified emails:
  - Dev Team → Developers  
  - DevOps → Infra & Automation  
  - QA → QA Engineers  
  - SRE → Reliability Engineers  
  - DB → Database Admins  

---

### ✅ Step 7: Grant Repository Access
- Configure **Read / Write / Admin** access:
  - Devs → Read/Write  
  - DevOps → Admin  
  - QA → Read  
  - DB → Read/Write  

---

### ✅ Step 8: Manage Access & Clean-up
- Convert repository visibility (**Public ↔ Private**).  
- Delete unused **users, teams, repos, or organization**.  
⚠️ **Note**: Deletion is permanent → Always **backup/transfer ownership** first!  

---

## 🔒 Additional Best Practices
- Enable **branch protection rules** (e.g., `main` branch cannot be force-pushed).  
- Enforce **pull request reviews** before merging.  
- Follow a **branching strategy**:
  - `main` → stable production code.  
  - `develop` → integration branch.  
  - `feature/*` → new features.  
  - `hotfix/*` → urgent fixes.  
- Use **GitHub Issues & Projects** for task tracking.  
- Setup **webhooks / GitHub Actions** for CI/CD automation.  
- Regularly review **audit logs** & permissions.  
- Use **service accounts** for automation instead of personal credentials.  
- Protect secrets using **GitHub Secrets**.  

---

## 🛠️ Basic Git & GitHub CLI Workflow

```bash
# Clone a repository
git clone https://github.com/<org>/<repo>.git

# Create a new branch
git checkout -b feature/my-feature

# Stage and commit changes
git add .
git commit -m "Added new feature"

# Push branch to GitHub
git push origin feature/my-feature

# Create a Pull Request (via GitHub UI or CLI)
