# GitHub Setup Guide & Source Code Management Overview

---

## What is GitHub?

GitHub is a cloud-based platform that provides **distributed version control** and **source code management (SCM)** using Git. It enables collaboration on code and project management across teams.

---

## Popular Communication Tools

These tools are often used alongside GitHub for effective team collaboration:

- Microsoft Teams
- Slack
- Skype for Business
- Discord
- Google Chat

---

## Source Code Management (SCM) Tools

Below is a list of widely used SCM tools:

- **GitHub**
- **Bitbucket**
- **GitLab**
- **SVN (Subversion)**
- **TVS**
- **CFS**

---

## GitHub Administration Steps

### ✅ Step 1: Create a GitHub Account

- **Email**: `kkeducationblr@gmail.com`
- **Password**: `P@a`
- **Username**: `kkeducation1234567`
- **Public URL**: [https://github.com/](https://github.com/)
- **Enterprise URL**: [https://airtel.github.com/](https://airtel.github.com/)

> ⚠️ Always use strong passwords and enable 2FA for security.

---

### ✅ Step 2: Log in to GitHub

- Navigate to [GitHub Login](https://github.com/login)
- Enter your credentials and access the dashboard.

---

### ✅ Step 3: Create an Organization

- **Organization Name**: `bsnl-4g-test`
- Add service accounts only (not personal emails):
  - ❌ `kkeducationblr@gmail.com`
  - ❌ `prasanth@bsnl.com`
  - ✅ `devops4g@bsnl.com`

---

### ✅ Step 4: Create Repositories

Create both **public** and **private** repositories under the organization.

- 🔒 Private Repo: [testing-private-repo](https://github.com/bsnl-4g-test/testing-private-repo)
- 🌐 Public Repo: [testing-public-repo](https://github.com/bsnl-4g-test/testing-public-repo)

---

### ✅ Step 5: Create Teams

Create specific teams for access and collaboration:

- **Dev Team**: `bsnl-dev-team`
- **DevOps Team**: `bsnl-DevOps-Team`
- (Optional): QA, SRE, DB, etc.

---

### ✅ Step 6: Add Users to Teams

Assign GitHub usernames or verified email addresses to each team:

- `bsnl-dev-team`: Developers
- `bsnl-DevOps-Team`: Infra and automation
- `bsnl-qa-team`: QA Engineers
- `bsnl-sre-team`: Site Reliability Engineers
- `bsnl-db-team`: DB Admins

---

### ✅ Step 7: Grant Repository Access to Teams

Configure repository permissions for each team:

- Read, Write, or Admin privileges as needed.
- Example:
  - Devs: Read/Write
  - DevOps: Admin
  - QA: Read
  - DB: Read/Write

---

### ✅ Step 8: Manage Access & Clean-up

- **Convert Repository Visibility**:
  - Public ↔ Private (can be changed anytime under repo settings)

- **Delete**:
  - Users
  - Teams
  - Repositories
  - Organization (if no longer required)

> Note: Deletion is permanent. Take backup or transfer ownership before deletion.

---

## Additional Best Practices

- Enable **branch protection rules**.
- Enforce **code reviews** before merging.
- Setup **webhooks** or **GitHub Actions** for automation.
- Regularly review **audit logs** for access tracking.
- Use **service accounts** for automation instead of personal credentials.

---

## Useful Links

- [GitHub Docs](https://docs.github.com/)
- [Git CLI Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [GitHub Actions](https://docs.github.com/en/actions)
