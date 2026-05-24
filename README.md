# 🏎️ Metal Wheels

<p align="center">
  <img src="Metal Wheels Logo.jpg" alt="Metal Wheels Logo" width="200" style="border-radius: 50%; box-shadow: 0 4px 15px rgba(0,0,0,0.25);" />
</p>

<p align="center">
  <strong>An AI-Free, Static HTML/CSS Showroom Masterpiece</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/Milestone-B.Tech%201st%20Year-9c27b0?style=for-the-badge" alt="Milestone" />
  <img src="https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey?style=for-the-badge" alt="License" />
</p>

---

## 📖 Project Overview

**Metal Wheels** is an elegant, pure static web portal displaying the world's most premium luxury and high-performance automobile brands—**BMW, Rolls-Royce, Porsche, and Lamborghini**. 

Originally built in **2023** during the author's **B.Tech 1st Year**, this project represents a significant milestone: **a fully handcrafted, AI-free coding project** built to master HTML5 structure, CSS styling, media integration, interactive client forms, and layout architecture.

The site is designed with a premium, sleek contrast aesthetic, offering a rich car card listing featuring autoplay looping preview videos, exact pricing, performance specifications, location mapping, and interactive review hooks.

---

## ✨ Features

- **🏆 Brand Showcases:** Fully styled, custom-designed sub-pages for **BMW**, **Rolls-Royce**, **Porsche**, and **Lamborghini**.
- **🎥 Autoplay Video Cards:** Each vehicle features an integrated, looping, muted MP4 video preview, providing a highly dynamic visual experience.
- **📊 Technical Specs:** Structured, clean tabular specs listing crucial vehicle parameters: engine displacement, top speed, battery capacity, range, and 0–100 km/h acceleration.
- **🗺️ Interactive Map:** Seamlessly integrated, interactive Google Maps location widget focused on HITEC City, Hyderabad.
- **📝 Review & Feedback Portal:** An interactive front-end rating and review submission system styled with custom form fields.
- **🎨 Custom Styling & Transitions:** High-fidelity interactive button hover scale animations, box-shadow transitions, and premium typography.

---

## 🛠️ Technology Stack

- **Markup:** Semantic HTML5 elements (`<header>`, `<nav>`, `<section>`, `<footer>`, `<video>`, `<form>`) for maximum accessibility and readability.
- **Styling:** Vanilla CSS3 featuring grid-like flexible layouts, scale transitions, shadow enhancements, and fully customized fonts.
- **Integrations:** Embed Google Maps API (iframe integration) and direct relative video looping.

---

## 📁 Repository Structure

We have kept all original 2023 source files intact in the root folder to preserve original paths and relative links, surrounding them with standard repository metadata.

```
Metal Wheels/
│
├── screenshot/                             # App screenshots
│   ├── Screenshot 2026-05-24 215349.png    # Homepage Home view
│   ├── Screenshot 2026-05-24 215419.png    # BMW specifications view
│   ├── Screenshot 2026-05-24 215444.png    # BMW gallery views
│   ├── Screenshot 2026-05-24 215456.png    # Rolls Royce showcase view
│   └── Screenshot 2026-05-24 215511.png    # Lamborghini cards view
│
├── docs/                                   # Project reports & architecture
│   └── reports/
│       ├── visibility_anti_copy.md         # Public vs Private / Anti-copy strategies report
│       └── promotion_audit.md              # Screenshot & Promo video marketing report
│
├── [Original B.Tech HTML Pages]
│   ├── index.html                          # Homepage & Main entrance
│   ├── BMW.html                            # BMW showcase page
│   ├── RollsRoyce.html                     # Rolls-Royce showcase page
│   ├── Porsche.html                        # Porsche showcase page
│   ├── Lamborghini.html                    # Lamborghini showcase page
│   ├── Contact.html                        # Contact page
│   ├── buy now.html                        # Mock Checkout / Buy Now page
│   ├── submit.html                         # Form Submission Landing Page
│   └── [more BMW/Lamborghini htmls...]     # Specific vehicle image portals
│
├── [Original B.Tech CSS Style Sheets]
│   ├── Metal Wheels.css                    # Main homepage style rules
│   ├── BMW.css                             # BMW custom branding styles
│   └── Lamborghini.css                     # Lamborghini custom branding styles
│
├── [Premium Media Assets]
│   ├── BMW M8.mp4                          # BMW M8 looping MP4 teaser
│   ├── BMW XM.mp4                          # BMW XM looping MP4 teaser
│   ├── BMW i7.mp4                          # BMW i7 looping MP4 teaser
│   └── Metal Wheels Logo.jpg               # Custom Metal Wheels branding logo
│
├── .gitignore                              # Prevents tracking caches, IDE configuration files
├── LICENSE                                 # Protective CC BY-NC-ND 4.0 License
├── CONTRIBUTING.md                         # Contribution guidelines & historical preservation
├── SECURITY.md                             # Security audit and reporting policy
└── CHANGELOG.md                            # Complete version history log
```

---

## 🖼️ Screenshots

### 1. Welcome to Metal Wheels (Main Landing)
![Home Page](screenshot/Screenshot%202026-05-24%20215349.png)

### 2. Premium Showroom (BMW Cards & Specifications)
![BMW View](screenshot/Screenshot%202026-05-24%20215419.png)

### 3. Detailed Gallery & Media
![Gallery View](screenshot/Screenshot%202026-05-24%20215444.png)

### 4. Interactive Feedback & Interactive Google Maps
![Map and Feedback Form](screenshot/Screenshot%202026-05-24%20215456.png)

### 5. High-Contrast Dark-Mode Showcases
![Lamborghini View](screenshot/Screenshot%202026-05-24%20215511.png)

---

## 🚀 Installation & Running Guide

Since this is a lightweight, pure static website, **no server environments, dependencies, node installations, or build tools are required.** 

To run the site locally:
1. Clone this repository to your local system:
   ```bash
   git clone https://github.com/kotojupreetham/Metal-wheels.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Metal-wheels
   ```
3. Open `index.html` directly in any web browser of your choice (Chrome, Safari, Firefox, or Edge):
   - Double-click `index.html` in your file explorer, OR
   - Run via terminal:
     ```bash
     # Windows (PowerShell)
     Start-Process index.html
     
     # macOS
     open index.html
     
     # Linux
     xdg-open index.html
     ```

---

## 🔮 Future Enhancements

While we are keeping the current project exactly as it was coded in 2023 to preserve its historical authenticity, future roadmap ideas for a v2 modern rebuild include:
- **Responsive Web Design (RWD):** Adding CSS media queries to scale optimally on all smartphones and mobile tablets.
- **Serverless Form Processing:** Connecting the review form to a serverless backend service like **Formspree** or **EmailJS** to collect live feedback.
- **Obfuscated Productions:** Injecting post-processors to minify code and obfuscate layout classnames to protect original designs from copycats.

---

## 🤝 Contribution Guidelines

This repository represents a preserved historical milestone. As such, direct pull requests, branch contributions, or modifications to the core codebase are closed. However, reviews, audits, and discussions are highly appreciated. 

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

---

## 📧 Contact Information

- **Developer:** Preetham Kotoju
- **Academic Milestone:** B.Tech Computer Science & Engineering (1st Year, 2023)
- **GitHub Profile:** [@kotojupreetham](https://github.com/kotojupreetham)
- **Repository URL:** [https://github.com/kotojupreetham/Metal-wheels](https://github.com/kotojupreetham/Metal-wheels)
