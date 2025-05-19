# 🚀 CodyBrookes.com — Static Portfolio Website with CI/CD

A clean, fast, and fully automated personal website built using **HTML/CSS** and deployed via a modern **CI/CD pipeline** using **GitHub Actions + AWS (S3, CloudFront, Route 53)**.

![Deployment Status](https://img.shields.io/github/actions/workflow/status/codybrookes/YOUR_REPO_NAME/deploy.yml?branch=main&label=deploy)

---

## 🧱 Project Overview

This repository contains the source code and infrastructure setup for my personal portfolio website, hosted at:

🌐 **[https://www.codybrookes.com](https://www.codybrookes.com)**

The site is 100% static and optimized for performance and simplicity.

---

## 🌐 Features & Architecture

- **Static Website**: Built using pure HTML/CSS
- **AWS S3**: Hosts static files with public access enabled
- **AWS CloudFront**: Distributes content globally with HTTPS and caching
- **Route 53**: Manages DNS for the `codybrookes.com` domain
- **GitHub Actions**: Handles continuous deployment from `main` branch

---

## ⚙️ CI/CD Pipeline Summary

- Push to `main` triggers an automated GitHub Actions workflow
- Syncs updated files to the S3 bucket (`codybrookes.com`)
- Invalidates CloudFront distribution to reflect changes instantly

### 🔐 GitHub Secrets Used
- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_REGION`

Workflow file:  
`.github/workflows/deploy.yml`

---

## 🗂 Repo Structure
├── index.html # Main website HTML
├── experience.html
├── projects.html
├── contact.html
├── thank-you.html
├── styles.css # Custom styles
├── .github/
│ └── workflows/
│ └── deploy.yml # GitHub Actions workflow
└── README.md # You're here


## 🛠 How I Use It

- **Update Content**: Edit HTML/CSS locally
- **Push to GitHub**: Changes are deployed automatically
- **Website Live**: Updated within ~1 minute globally via CloudFront

---

## ✨ Highlights

- 📦 Fully automated pipeline from commit to deploy
- ☁️ Real-world AWS infrastructure setup (IAM, S3, CloudFront, Route 53)
- 🔐 Secure secrets management via GitHub
- ⚡ Ultra-fast global performance with CDN and HTTPS

---

## 🤝 Let's Connect

This site is just the start of a broader portfolio — more projects, automation, and infrastructure coming soon.

Built and maintained by **Cody Brookes** 💻  
Reach me at: [https://www.codybrookes.com#contact](https://www.codybrookes.com#contact)

---
