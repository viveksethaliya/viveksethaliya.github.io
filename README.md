# DNS Basics Project

This project was created to learn and practice the basics of DNS by setting up a custom domain name with both **GitHub Pages** and a **cloud instance** (AWS instead of DigitalOcean).

---

## Requirements
- A purchased custom domain name (.xyz from GoDaddy).
- A static site deployed on **GitHub Pages**.
- A static site hosted on an **AWS EC2 instance**.
- Proper DNS records pointing the domain name to both GitHub Pages and AWS.

---

## Task #1 - Custom Domain for GitHub Pages

### Steps I Took:
1. Purchased a `.xyz` domain from **GoDaddy**.
2. Created a repository on GitHub with my static website files.
3. Configured **GitHub Actions** to build and deploy my site to **GitHub Pages**.
4. In the repository settings → **Pages**, I set the deployment branch and confirmed the site was live on `username.github.io/repository`.
5. Updated my **GoDaddy DNS settings**:
   - Added a **CNAME record** pointing my domain (`www.mydomain.xyz`) to my GitHub Pages domain (`username.github.io`).
   - (Optional) Added an **A record** for the root domain (`mydomain.xyz`) pointing to GitHub Pages IPs.
6. Verified that `mydomain.xyz` correctly forwarded to my GitHub Pages site.

---

## Task #2 - Custom Domain for AWS Instance

Instead of using DigitalOcean, I hosted my static site on **AWS S3**.

### Steps I Took:
1. Launched an **AWS S3 bucket**
   configured the S3 bucket and routed it with aws route 53 tool for my godaddy doomain
 --------------------------------
 Project from: https://roadmap.sh/projects/basic-dns
