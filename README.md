# Sameer Sirsath — Professional AI & Engineering Portfolio

A modern, mobile-optimized, ultra-responsive developer & professional portfolio web application crafted specifically for **Sirsath Sameer Sahebrao** (3rd Year B.Tech CSE - AI & ML at **MIT Academy of Engineering, Pune**). Built for seamless embedding into **Google Sites** (Full-Page Embed or standard Embed blocks) as well as standalone hosting.

---

## 🌟 Highlights & Features

- ⚡ **Zero-Build, Single-File Bundle**: Everything (CSS, SVG icons, animated JS) is contained in `index.html`. No Node.js build step or complex setup needed.
- 📱 **Mobile-First Touch View**: Glassmorphism mobile drawer, 48px touch targets, quick contact bar (Call/Email/LinkedIn), and responsive timeline layouts.
- 🎨 **Executive Visual Design**: Modern glassmorphism, ambient gradient glow orbs, subtle grid texture, and fluid typography.
- 🔄 **Silky 7-Tab Navigation**:
  - **Home**: Dynamic typing animation, student KPI metrics, profile card, and core technical pillars.
  - **Professional Journey**: Sagveek Technologies AI/ML internship, campus technical leadership, and research/hackathon milestones.
  - **Projects**: Filterable gallery featuring the deployed **AI Chatbot for Persons with Disabilities** on Render, **Anti-Sleeping System for Drivers**, and **Legal Lens**.
  - **Educational Journey**: Vertical milestone timeline for MITAOE Pune (B.Tech AI & ML), Shri Sant Dnyaneshwar Jr College, and Ansooya Vidya Mandir.
  - **Certifications & Achievements**: Issuer badges & verify links for IIT Madras Pravartak (94/100), AWS GenAI, Cisco Python, Oracle SQL, and Avishkar Zonal honors.
  - **Skills & Tech Stack**: Interactive categorized skill chips.
  - **Get In Touch**: 1-click clipboard copy for email & phone, social media buttons, and direct-to-inbox contact form.
- 🌙 **Dark & Light Mode**: Smooth theme toggle with persistent CSS tokens.
- 🛡️ **Google Sites Iframe Hardened**: All external links use `target="_blank"` and `rel="noopener noreferrer"`, guaranteeing zero iframe sandboxing breakage.

---

## 🚀 How to Embed into Google Sites (Step-by-Step)

Google Sites provides two great ways to embed this portfolio:

### Method 1: "Full Page Embed" (Recommended - Cleanest Look)

1. Open your site on [Google Sites](https://sites.google.com/).
2. On the right-hand panel, switch to the **Pages** tab.
3. Hover over the **`+`** (Add page) button at the bottom and select **"Full page embed"** (the `< >` icon).
4. Name your page (e.g. `Portfolio` or `Home`) and click **Done**.
5. On the new page canvas, click the **"Add embed"** button in the center.
6. In the pop-up modal, select the **"Embed code"** tab.
7. Open `index.html` from this folder, **select all (Ctrl+A / Cmd+A)**, **copy (Ctrl+C / Cmd+C)**, and paste it into the code box.
8. Click **Next**, preview the page, and click **Insert**.
9. Click **Publish** in the top right.

---

### Method 2: Standard Embed Block (Full Canvas Drag)

If you prefer inserting it inside an existing Google Sites page:
1. In the right panel under **Insert**, click **Embed** (`< >`).
2. Choose **Embed code**.
3. Paste the contents of `index.html` and click **Next** then **Insert**.
4. Drag the blue corner bounding boxes of the embed block all the way to the edges of the page width and stretch down the height until it fills your desired view smoothly.
5. Click **Publish**.

---

### Method 3: Host on GitHub Pages & Embed by URL (Alternative)

If you'd like to update your portfolio code via GitHub without touching Google Sites again:
1. Push `index.html` to a public GitHub repository.
2. Go to repository **Settings > Pages > Deploy from branch (main / root)**.
3. Copy your live URL (e.g., `https://yourusername.github.io/portfolio`).
4. In Google Sites, click **Insert > Embed > By URL**, paste your GitHub Pages link, and click **Insert**.

---

## ✏️ How to Personalize Your Information

All personal details in [index.html](file:///f:/portfolio/index.html) are clearly marked with `<!-- EDIT: ... -->` comments. You can open `index.html` in VS Code or any text editor and search for `EDIT:` to customize:

### 1. Name, Title & Bio
- Profile details are customized for **Sameer Sirsath**, 3rd-year B.Tech student in Computer Science (AI & ML) at MIT Academy of Engineering, Pune.
- For the typing animation at the top, edit the `roles` array near the bottom of `index.html`:
  ```javascript
  const roles = [
    "AI & ML Enthusiast.",
    "3rd Year B.Tech CSE (AI & ML).",
    "Python & Backend Developer.",
    "RAG & Generative AI Builder.",
    "Data Analyst & Problem Solver."
  ];
  ```

### 2. Profile Photo
- Find `avatar-img`:
  ```html
  <img src="..." alt="Sameer Sirsath" class="avatar-img">
  ```
  Replace the `src` with a URL to your photo (e.g., GitHub avatar URL, LinkedIn photo URL, or Imgur link).

### 3. Professional Journey / Experiences
- Scroll down to `<section id="pane-experience">`.
- To add another internship or project role, copy any `<div class="experience-item">...</div>` and paste it at the top of `.experience-container`.
- Update the role title, company name, date pill, and bullet points.

### 4. Projects
- Scroll down to `<section id="pane-projects">`.
- Currently features the live deployed **AI Chatbot for Persons with Disabilities** on Render, **Anti-Sleeping System for Drivers**, **Medical Devices RAG System**, and **Legal Lens**.
- Update project links, demo URLs, or add new projects using the `<article class="project-card">` template.

### 5. Educational Journey & Milestones
- Scroll down to `<section id="pane-education">`.
- Configured with MITAOE Pune (B.Tech AI & ML, CGPA: 7.64), Shri Sant Dnyaneshwar Jr College (67.33%), and Ansooya Vidya Mandir (95.80%).

### 6. Certifications & Achievements
- Scroll down to `<section id="pane-certifications">`.
- Displays IIT Madras Pravartak (94/100), AWS Generative AI, Cisco Python, Oracle SQL, and Avishkar Zonal research honors.

### 7. Direct-to-Inbox Contact Form & Details
- **Step 1**: In `index.html`, recipient email is set to:
  ```javascript
  const RECIPIENT_EMAIL = "sameersirsath2503@gmail.com";
  ```
- **Step 2 (One-Time Activation)**:
  - Submit the form once on your site.
  - You will receive a single verification email from **FormSubmit** asking you to confirm your email.
  - Click the **"Activate Form"** button in that email once.
  - Done! Every inquiry submitted through your portfolio will land **instantly and directly in your email inbox**, with full sender details and message contents!
- **Step 3 (Cards Info)**:
  - In `<section id="pane-contact">`, contact cards are populated with `sameersirsath2503@gmail.com`, `+91-8793218900`, Pune location, and your LinkedIn profile link.

---

## 💻 Local Testing & Preview

To preview the portfolio locally before embedding:
1. Double-click [index.html](file:///f:/portfolio/index.html) to open directly in Chrome, Edge, or Firefox.
2. Or use Python's built-in HTTP server:
   ```bash
   python -m http.server 8080
   ```
   and navigate to `http://localhost:8080`.
