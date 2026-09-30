# Personal Developer Portfolio

A modern, responsive and minimal developer portfolio website built from scratch using **HTML5 and Tailwind CSS**.

The project showcases a developer profile through a structured portfolio website containing an introduction, technology stack, selected projects, experience timeline, contact section and a dedicated technical blog page.

The project was built as a hands-on frontend project to practice **Tailwind CSS, responsive design, custom styling, animations and multi-page website development**.

---

## 🌐 Live Website

**Portfolio:**  
https://its-lnv.github.io/html-tailwind-portfolio/

---

## 📌 About The Project

This project is a personal developer portfolio designed with a clean, minimal and professional interface.

The main portfolio page presents:

- Developer introduction
- Technology stack
- Selected projects
- Professional experience
- Contact information
- Social links

The project also contains a separate blog page where technical concepts are explained in a beginner-friendly format.

The current blog article focuses on **Docker and containerization**, covering topics such as Docker containers, images, Dockerfiles, Docker Compose and Containers vs Virtual Machines.

---

## ✨ Features

### Portfolio

- Responsive hero section
- Developer introduction
- "Open to new opportunities" status
- Project showcase
- Technology stack section
- Experience timeline
- Contact section
- Email contact card
- Social media buttons
- Responsive layout

### Blog

- Dedicated technical blog page
- Blog category and reading-time information
- Beginner-friendly article structure
- Sticky table of contents on larger screens
- Multiple technical sections
- Containers vs Virtual Machines comparison
- Docker concepts explained through examples
- Docker Compose explanation
- Beginner Docker learning roadmap

### UI & Design

- Minimal developer-focused design
- Responsive layouts
- Dark/light color scheme
- Custom color variables
- Amber accent color
- Custom typography
- Google Fonts integration
- Smooth scrolling
- Hover effects
- CSS transitions
- Fade-in animations
- Custom scrollbar
- Responsive cards and sections

---

## 🛠️ Technologies Used

### Frontend

- HTML5
- Tailwind CSS
- CSS

### Fonts

- Inter
- Playfair Display
- JetBrains Mono

### Other

- Google Fonts
- SVG icons
- Tailwind CSS animations and utilities

---

## 🎨 Design System

The project uses custom CSS variables to maintain consistent colors throughout the website.

### Main Design Tokens

- Surface
- Surface Card
- Surface Solid
- Code Surface
- Primary Text
- Secondary Text
- Muted Text
- Borders
- Accent
- Accent Background
- Accent Border
- Navbar Background

Tailwind's `@theme` configuration is also used to define custom font families.

```css
@theme {
    --font-sans: 'Inter', ui-sans-serif, system-ui, sans-serif;
    --font-serif: 'Playfair Display', ui-serif, Georgia, serif;
    --font-mono: 'JetBrains Mono', ui-monospace, 'Courier New', monospace;
}
```

---

## 📄 Pages

### 1. Portfolio — `index.html`

The main page of the project.

It contains:

#### Hero Section

Introduces the developer and provides navigation to projects and contact sections.

#### Tech Stack

Displays frontend, backend and DevOps technologies.

#### Selected Work

Contains project cards with:

- Project name
- Project category
- Description
- Technologies used
- Hover interaction

#### Experience

A timeline-style section showing professional experience.

#### Contact

Provides:

- Email
- GitHub
- LinkedIn
- Twitter/X

---

### 2. Blog — `blog.html`

A dedicated technical blog page.

#### Article

**Docker Explained: Why Every Developer Should Learn Containers**

The article covers:

1. The "Works on My Machine" problem
2. What is Docker?
3. Containers vs Virtual Machines
4. Docker Images
5. Docker Containers
6. Dockerfiles
7. Docker Hub
8. Docker Compose
9. Why teams use Docker
10. Where beginners should start

The blog also includes a sidebar table of contents for easier navigation.

---

## 📁 Project Structure

```text
portfolio-website/
│
├── index.html
├── blog.html
│
├── input.css
├── output.css
│
├── package.json
├── package-lock.json
│
├── .gitignore
│
└── node_modules/
```

### File Description

| File | Purpose |
|------|---------|
| `index.html` | Main portfolio page |
| `blog.html` | Technical blog page |
| `input.css` | Tailwind CSS source file and custom styles |
| `output.css` | Generated Tailwind CSS file |
| `package.json` | Project dependencies and configuration |
| `package-lock.json` | Locked dependency versions |
| `.gitignore` | Files/folders excluded from Git |

---

# ⚙️ How To Run The Project

There are two simple ways to run this project.

---

## Method 1 — Run Directly

If `output.css` is already generated and present in the project:

### Step 1 — Clone the repository

```bash
git clone https://github.com/lakshminarayanverma91-bot/portfolio-website.git
```

### Step 2 — Move into the project directory

```bash
cd portfolio-website
```

### Step 3 — Open the website

Open:

```text
index.html
```

in your browser.

You can also use the **Live Server** extension in VS Code.

---

# Method 2 — Run Tailwind CSS in Development

Use this method if you want to modify Tailwind classes/CSS and automatically regenerate `output.css`.

## Step 1 — Clone the repository

```bash
git clone https://github.com/lakshminarayanverma91-bot/portfolio-website.git
```

## Step 2 — Enter the project directory

```bash
cd portfolio-website
```

## Step 3 — Install dependencies

```bash
npm install
```

This installs the dependencies listed in `package.json`.

## Step 4 — Start Tailwind

Run:

```bash
npx @tailwindcss/cli -i ./input.css -o ./output.css --watch
```

This command:

- Reads styles from `input.css`
- Processes Tailwind CSS
- Generates `output.css`
- Watches for changes

Whenever you modify your HTML or CSS, Tailwind can regenerate the output CSS automatically.

## Step 5 — Open the website

Open:

```text
index.html
```

in your browser.

For development, using **Live Server in VS Code** is recommended.

---

# 🔄 Development Workflow

A typical workflow for editing this project is:

```text
Edit HTML / CSS
       ↓
Tailwind CLI watches files
       ↓
output.css gets updated
       ↓
Browser reloads
       ↓
Changes appear on website
```

Keep the following command running while developing:

```bash
npx @tailwindcss/cli -i ./input.css -o ./output.css --watch
```

---

# 🎨 Custom CSS

The `input.css` file contains both Tailwind configuration and custom CSS.

It includes:

- Tailwind import
- Google Fonts
- Custom font configuration
- CSS variables
- Dark/light color scheme
- Base styles
- Scrollbar customization
- Custom animations

Example:

```css
@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(22px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}
```

The animation is used throughout the portfolio to create subtle entrance effects.

---

# 📱 Responsive Design

The website is designed to work across different screen sizes.

Tailwind responsive utilities are used to adapt:

- Typography
- Navigation
- Project grids
- Experience sections
- Spacing
- Blog layout
- Content width

The project uses responsive breakpoints such as:

```text
sm
md
lg
xl
```

---

# 📚 Learning Outcomes

This project helped me practice and understand:

- Tailwind CSS fundamentals
- Utility-first CSS
- Responsive web design
- Tailwind responsive breakpoints
- Custom CSS variables
- Tailwind `@theme`
- Custom fonts
- CSS animations
- Hover states
- Transitions
- Multi-page website structure
- Responsive project cards
- Timeline layouts
- Blog page design
- Technical content presentation
- Tailwind CLI workflow

---

# 🚀 Future Improvements

Possible improvements for future versions include:

- Add JavaScript-based interactions
- Add a mobile navigation menu
- Connect real project links
- Add actual GitHub and LinkedIn URLs
- Add a downloadable resume
- Add more technical blog posts
- Add a functional contact form
- Add project filtering
- Improve accessibility
- Add more interactive animations
- Add a dedicated projects page

---

# 🔗 Links

### Live Website

https://its-lnv.github.io/html-tailwind-portfolio/

### GitHub Repository

https://github.com/its-lnv/html-tailwind-portfolio

---

## 👨‍💻 Author

**Laxmi Narayan**

Developer | Computer Science Student

---

## 📄 License

This project is created for learning, practice and portfolio purposes.
