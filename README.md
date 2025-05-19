# 🚀 CodyBrookes.com

A personal portfolio website built with HTML/CSS, hosted on **AWS S3 + CloudFront**, and deployed automatically using **GitHub Actions CI/CD**.

![Deployment Status](https://img.shields.io/github/actions/workflow/status/codybrookes/codybrookes-digital-portfoliosite/deploy.yml?branch=main&label=deploy)

---

## 🔍 Overview

This site showcases my work, passion for technology, and projects in cloud, automation, and full-stack development. It's designed for speed, simplicity, and scalability.

---

## 🧱 Tech Stack

| Tech         | Purpose                          |
|--------------|----------------------------------|
| HTML/CSS     | Static website content           |
| AWS S3       | Static site hosting              |
| CloudFront   | CDN + HTTPS + caching            |
| GitHub       | Source control                   |
| GitHub Actions | CI/CD for automatic deployment |

---

## ⚙️ CI/CD Pipeline Details

Every push to the `main` branch triggers an automated deployment via [GitHub Actions](https://github.com/features/actions).

### 📦 Workflow Steps:

1. **Checkout** the latest code from the repo
2. **Authenticate** with AWS using encrypted GitHub secrets
3. **Sync** the site to S3 using `aws s3 sync`
4. **Invalidate CloudFront** cache to reflect the latest changes

### 🛡️ Secrets Used

Secrets are stored securely in GitHub under:
- `AWS_ACCESS_KEY_ID`
- `AWS_SECRET_ACCESS_KEY`
- `AWS_REGION`

---

## 🗂 Directory Structure

```bash
.github/workflows/deploy.yml   # GitHub Actions workflow
index.html                     # Main site HTML
styles.css                     # Stylesheet
experience.html
projects.html
contact.html
thank-you.htm
...

## 🌐 Live Site
https://www.codybrookes.com

Hosted via AWS S3 with CloudFront, using custom domain + HTTPS.
