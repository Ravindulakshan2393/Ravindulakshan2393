# 📘 GitHub Profile README — Maintenance & Customization Guide

This guide provides step-by-step instructions on how to maintain, update, and customize your GitHub Profile README (`README.md`), custom SVG header/footer banners, tech stack badges, and analytics cards.

---

## 📂 Repository File Structure

| File / Directory | Description |
| :--- | :--- |
| [`README.md`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/README.md) | **Primary Profile File** rendered on your GitHub profile homepage (`https://github.com/Ravindulakshan2393`). |
| [`assets/header.svg`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/assets/header.svg) | Custom SVG gradient header banner displaying your name and degree subtitle. |
| [`assets/footer.svg`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/assets/footer.svg) | Custom SVG wave graphic for the bottom finish of your profile. |
| [`preview.html`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/preview.html) | Local HTML file to preview your profile live in Chrome/Edge without pushing to GitHub. |
| [`DOCUMENTATION.md`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/DOCUMENTATION.md) | This maintenance and customization guide. |

---

## 🚀 How to Preview Your Profile Locally (Without Pushing)

### Method 1: Using `preview.html` in Web Browser
1. Open [`preview.html`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/preview.html) in your browser (double-click in File Explorer or open in Chrome).
2. Whenever you edit `README.md`, refresh your browser page (**`F5`** or **`Ctrl + R`**) to see live updates instantly.

### Method 2: VS Code Built-in Preview
1. Open [`README.md`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/README.md) in VS Code.
2. Press **`Ctrl + Shift + V`** (or **`Ctrl + K`**, then **`V`** for side-by-side view).

---

## ✏️ How to Customize & Update Content

### 1. Updating Header Name & Subtitle
- Open [`assets/header.svg`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/assets/header.svg).
- Edit the text inside line 29:
  ```xml
  <text class="sub" x="450" y="115" text-anchor="middle"
        font-family="'Segoe UI', Ubuntu, 'Helvetica Neue', Sans-Serif"
        font-size="17" fill="#8b949e">YOUR NEW SUBTITLE HERE</text>
  ```

### 2. Updating Animated Typing Banner Text
- Open [`README.md`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/README.md).
- Edit the `lines=` query parameter in the typing SVG URL:
  ```markdown
  lines=Hey+there!+I'm+Sadeepa+Lakshan;BSc.+(Hons)+IT+%26+Management+Undergrad+%40+UoM;Aspiring+Software+Engineer;Full+Stack+Development+Enthusiast;Building+ideas+into+reality
  ```
  *(Note: Replace spaces with `+` and `&` with `%26`)*.

### 3. Updating the YAML "About Me" Block
- Edit the YAML block directly in [`README.md`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/README.md):
  ```yaml
  name        : Sadeepa Lakshan
  degree      : BSc. (Hons) Information Technology & Management [Undergraduate @ University of Moratuwa]
  interests   : Software Engineering ⚡ Full-Stack Web Development ⚡ Database Systems ⚡ IoT
  goal        : Secure a Software Development Internship & build impactful software solutions
  status      : Seeking internship opportunities & open to technical collaborations 🚀
  quote       : "Life is full of choices… choose wisely!"
  ```

---

## 🛠️ How to Add / Remove Tech Badges (Shields.io)

Badges use **Shields.io** syntax.

### Syntax Template:
```markdown
![Badge Title](https://img.shields.io/badge/LABEL-HEXCOLOR?style=for-the-badge&logo=LOGONAME&logoColor=white)
```

### Examples:
- **TypeScript**: `![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)`
- **Python**: `![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)`
- **Docker**: `![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)`

---

## 📂 How to Add Projects in the Future

When you are ready to showcase your projects, add a table section to [`README.md`](file:///d:/Projects/SoftProject/GitHub/Ravindulakshan2393/README.md):

```markdown
## 📂 Featured Projects

| Project | Description | Tech Stack | Repository |
| :--- | :--- | :--- | :---: |
| 🚛 **ConTrack** | Container Transport Logistics Management System. | `React` `Node.js` `PostgreSQL` | [🔗 View Code](https://github.com/Ravindulakshan2393) |
| 📟 **Abacus Genius 1.0** | Arduino educational device with keypad & LCD. | `Arduino Mega` `ESP8266` | [🔗 View Code](https://github.com/Ravindulakshan2393/Abacus-Genius-1.0) |
```

---

## 🔄 How to Commit & Push Updates to GitHub

Run these commands in your VS Code Terminal (`Ctrl + ~`):

```bash
# 1. Stage all changes
git add .

# 2. Commit changes with a descriptive message
git commit -m "Update profile README info and skills"

# 3. Push live to GitHub
git push origin main
```

---

## 💡 Troubleshooting & FAQ

- **Image / Card Broken on GitHub?**  
  GitHub caches external badge images. If an image doesn't update immediately after pushing, wait 2–3 minutes or do a hard refresh (**`Ctrl + F5`**).
- **Social Link Not Opening Mail Client?**  
  Ensure the mail link is formatted as `mailto:your-email@gmail.com`.
