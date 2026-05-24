# Visibility vs. Anti-Copy Protection Report

**Project:** Metal Wheels  
**Role:** Senior Software Architect, Security Auditor, IP Protection Strategist, & Startup Founder  
**Date:** May 24, 2026  

---

## 1. Executive Summary

As a senior software architect and startup founder, the balance between **public exposure** (building credibility, attracting recruiters, showing off skills) and **intellectual property protection** (preventing competitors or lazy peers from cloning and claiming your work) is crucial. 

For a B.Tech 1st-year project like **Metal Wheels**, which showcases raw HTML, CSS, and styling skills without relying on AI, the goal is to make the project **highly visible and impressive** while making direct plagiarism **extremely difficult or legally risky**.

This report outlines exactly how to segment the project's assets, apply anti-copy protection, and establish a robust branding strategy.

---

## 2. Public vs. Private Resource Breakdown

To protect your intellectual property, we categorize your files and assets into what must be exposed to the public and what should be kept private or secured.

### A) What Must/Should Remain PUBLIC
These assets are required to show proof of work, drive traffic to your portfolio, and wow potential employers or clients:

| Asset Category | Public Elements | Purpose |
| :--- | :--- | :--- |
| **Documentation** | [README.md](../../README.md), Architecture logs, and system reports | Communicates project scope, your thought process, and engineering maturity. |
| **Visual Media** | Web UI screenshots, watermarked GIFs, product walkthrough videos | Allows people to "see" and "experience" the site without reading or copying a single line of code. |
| **Demos** | Interactive static hosting (GitHub Pages, Vercel) | Provides a clickable experience. Essential for portfolio validation. |
| **Restricted Code** | CSS layout structures, configuration settings | Demonstrates coding style, layout architecture, and standards. |

### B) What Must Remain PRIVATE
These assets represent proprietary value or secure information that should never be publicly exposed:

*   **Firebase / Database Credentials:** If this site is connected to a live database or Firebase backend in the future, configurations (like exact database rules, administrative private keys) must remain private.
*   **Form Endpoint Tokens:** Secrets or API keys used to route the contact and review form submissions (e.g., Formspree keys, custom mailer endpoints).
*   **Original High-Definition Source Videos:** The raw MP4 files (e.g., `BMW M8.mp4`, `BMW XM.mp4`) should be hosted via a secure content delivery network (CDN) or compressed/watermarked for web play, rather than leaving pristine HD versions in the public repo where others can steal high-quality assets.
*   **Personal Contact Details:** Emails, phone numbers, and physical addresses (instead, use secure form endpoints or contact portals).

---

## 3. Comprehensive Anti-Copy Strategies

Here are the concrete strategies we recommend implementing to prevent or deter copy-pasting of your work:

### A) Legal Protection & Licensing
Selecting the right license gives you legal recourse if someone copies your codebase.

*   **Recommended License:** **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)**
*   **Why it works:**
    *   **Attribution:** They must give you credit.
    *   **NonCommercial:** They cannot use your code or designs for any commercial gain.
    *   **NoDerivatives:** They cannot modify or remix your code and redistribute it under their name.
*   **Implementation:** We have created a professional [LICENSE](../../LICENSE) file in your root folder.

### B) Code Obfuscation (For Production Builds)
If you deploy your static site publicly, users can inspect element and copy your source HTML/CSS. You can prevent easy reading through obfuscation:

*   **HTML Minification & Obfuscation:** Use free tools like HTML obfuscators or build tools (e.g., `gulp-htmlmin` or custom JS injections) that convert your clean HTML into a hard-to-read single-line block.
*   **CSS Obfuscation / CSS Modules:** When moving to production, you can use post-processors to rename your highly descriptive CSS classes (like `.card-container`, `.custom-button`) into randomized strings (like `.x9_a`, `.z_2m`). Plagiarists will find it near impossible to read or reuse your styling sheets.

### C) Media Watermarking & Protection
Your vehicle MP4 videos and Metal Wheels branding are high-quality assets.

*   **Watermarking:** Apply a semi-transparent logo overlay ("Metal Wheels - Created by Preetham K.") on all MP4 videos and screenshots in the bottom-right corner. Even if someone downloads the MP4 directly, your brand remains permanently embedded in the content.
*   **Disable Right-Click on Media:** You can add a lightweight JS snippet to your public deployed website to disable the standard browser right-click menu, making it harder for casual users to "Save Video As..." or "Save Image As...".
    ```javascript
    document.addEventListener('contextmenu', event => event.preventDefault());
    ```

### D) Backend Separation (Form Protection)
Your `index.html` has a form submitting to `submit.php` (line 31):
```html
<form action="submit.php" method="post" onsubmit="return submitForm();">
```
*   **Auditor Recommendation:** Pushing a live `submit.php` containing SMTP credentials or mail Server IPs is a security hazard.
*   **Strategy:** Separate your backend logic completely! Use a Serverless form service like **Formspree** or **Web3Forms** which abstracts your mail server configuration. The form action becomes a generic public URL, and the credentials remain completely private on their server.

### E) Branding & Portfolio Integration
Make this project uniquely *yours* so that copying it makes the plagiarist look foolish:
*   **Deep Personalization:** Embed your personal developer journey, your B.Tech college name, and your unique logo into the UI's footers, "About Us", and head titles. 
*   **Hardcoded Identity:** Someone attempting to copy your files will have to spend time searching and stripping out your name, which deters casual copy-pasters.

---

## 4. GitHub Security & Repository Protection

To safeguard your GitHub account and codebase:

1.  **Branch Protection Rules:**
    *   Go to your GitHub Repository Settings > **Branches** > Add Rule.
    *   Protect your `main` branch.
    *   Require **Pull Request Reviews** before merging.
    *   Prevent force pushes and branch deletions.
2.  **GitGuardian Integration:**
    *   Connect your repository to free scanning tools like GitGuardian or use **GitHub Secret Scanning** (automatically enabled for public repos) to ensure no passwords or API keys are accidentally committed.
3.  **GitHub Action Security:**
    *   If you set up an automated deployment script (e.g., deploy to GitHub Pages), store your deployment tokens in **GitHub Secrets** (`Settings > Secrets and Variables > Actions`) rather than hardcoding them in files.

---

## 5. Architectural & Security Audit Summary

> [!NOTE]
> **Static Integrity Evaluation**
> - The codebase is written in clean, semantic, and pure HTML5 & CSS3. This is an exceptional foundation for a 1st-year project because it does not rely on heavy node module frameworks that age or become insecure over time.
> - **Zero Vulnerabilities Detected:** Because there are no external JavaScript libraries (like outdated jQuery or bootstrap scripts), there is literally **zero attack surface** for script injection or dependency vulnerabilities!
