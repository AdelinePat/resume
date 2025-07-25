# 🎓 Clara Moreau – Fake Resume

> *This project is part of a certification training in HTML, CSS, and Sass from Dyma. It simulates a complete resume website using semantic HTML5, modular SCSS, and modern development workflow tools like Node.js and npm.*

---

## 📌 Project Overview

This fake resume was created as a front-end integration exercise to apply and demonstrate knowledge of:

- Semantic HTML5 structure
- Modern CSS practices using SCSS (Sass)
- Responsive design with media queries
- Utility-first class architecture (`.mb-6`, `.title`, etc.)
- Sass mixins, inheritance, and variables for scalable styles
- A modular architecture to separate concerns and ensure maintainability

While the content (Clara Moreau) is entirely fictional, the techniques and workflow mimic a real-world development process.

---

## ⚙️ Environment Setup

To compile SCSS into CSS, this project uses [Node.js](https://nodejs.org/) and `npm` to install Sass locally.

### ✅ Prerequisites

- Node.js installed on your machine

### 🧰 Installation Guide

#### Windows

1. Download the Node.js installer (`.msi`) from the [official Node.js website](https://nodejs.org/)
2. Follow the setup instructions and ensure `npm` is added to your system PATH

#### Linux

```bash
sudo apt update
sudo apt install nodejs npm
```

#### Project Setup

Once Node.js is installed:

```bash
# Clone the repository
git clone https://github.com/AdelinePat/resume
cd resume

# Initialize the project
npm init -y

# Install Sass locally
npm install sass -y

```

> ☝️ `node_modules` and `package-lock.json` are ignored in this project via `.gitignore` to keep the repo clean. You can reinitialize the environment by running the commands above.

#### SCSS Compilation

To compile your styles:

```json
// In package.json:
"scripts": {
  "sass": "sass -w style/scss:style/css"
}
```
then run
```bash
npm run sass
```

This command watches the SCSS file and automatically compiles to `style.css` on every change.

## 🗂️ Project Structure

```
📁 clara-moreau-fake-resume/
├── index.html
├── img/
│   └── profile.jpg
└── style/
    ├── css/
    │   └── style.css        # Compiled output
    └── scss/
        ├── _animations.scss
        ├── _base.scss       # Base styles (e.g., html, body, h1...)
        ├── _classes.scss    # Component-like classes (e.g., .bar-skill)
        ├── _generic.scss    # Utility and helper classes (e.g., .title, .mb-6)
        ├── _media_queries.scss
        ├── _mixin.scss      # Reusable mixins (e.g., for bar-skill)
        ├── _reset.scss
        ├── _variables.scss  # CSS variables and SCSS maps
        └── style.scss       # Main SCSS file that imports everything
```
## 🧠 Learning Highlights

- **SCSS Modularity**: Each file handles a specific layer of the design (reset, layout, utilities, components).
- **Mixins & Inheritance**: Complex components like skill bars are created using mixins to keep the code DRY and scalable.
- **Responsive Design**: Custom media query mixins make it easy to adapt layout and typography to different screen sizes.
- **Utility-First Classes**: Small reusable classes (`.mb-6`, `.text-hint`, etc.) help speed up development and keep the HTML lean.

## 💡 About This Project

This resume is intentionally fake and marked clearly as such in the UI. Its purpose is educational:

> *"Ce projet a été réalisé dans le cadre du cours Dyma : ceci est un faux CV destiné à l'apprentissage."*

Feel free to explore or adapt it as a boilerplate for similar projects using SCSS.

## 🚀 What's Next?

This resume is part of a broader front-end learning journey. The next steps include:

- Creating a real portfolio with real content
- Learning JavaScript (DOM manipulation and fetch API)
- Transitioning to React for component-based UI
- Implementing CI/CD and Docker for automated deployment

Stay tuned ✨

## 📄 License

This project is shared for educational purposes and is not intended for commercial use.