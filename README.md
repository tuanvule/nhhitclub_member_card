# 🌟 Mini Team Project for Coding Club

This is a super basic teamwork project to help members in your coding club get familiar with version control (GitHub), teamwork workflows, and the joy of seeing each other's code and progress.

## 🎯 Project Idea

A shared webpage where each member creates their own card (like a mini-profile or fun showcase) using HTML + CSS. These cards are displayed on a shared homepage via `<iframe>`.

---

## 📁 Folder Structure

```
project-root/
├── index.html          # Main homepage
├── style.css           # Styling for layout and animations
├── members/
│   ├── alice.html      # Each member adds their own HTML file
│   ├── bob.html
│   └── ...
└── README.md           # This file
```

---

## ✨ Features

- Members add cards by editing `members/[name].html`
- Homepage (`index.html`) will display everyone's cards in a flex layout
- Hovering a card will slightly zoom it for effect
- Clicking a card will expand it to fullscreen using a modal-style effect

---

## 🔧 How to Use

1. **Clone the repo:**
   ```bash
   git clone https://github.com/your-org/mini-team-project.git
   ```

2. **Add your card:**
   - Go to the `members/` folder
   - Create a file named `yourname.html`
   - Put any HTML content you like (images, text, animations...)
   - Keep the layout inside 250x200px

3. **Test locally:**
   ```bash
   open index.html  # or use Live Server extension in VSCode
   ```

4. **Commit & Push:**
   ```bash
   git add members/yourname.html
   git commit -m "Add my member card"
   git push origin main
   ```

---

## 🪄 Card Zoom & Focus

### On Hover

Cards automatically zoom when hovered.

CSS used:
```css
iframe:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  z-index: 1;
}
```

### On Click - Fullscreen

Each card can be expanded fullscreen on click.

Code logic (JavaScript):
- On click: clone the `iframe`, enlarge it, and overlay it on screen
- Click outside or press `ESC` to close

---

## 🤝 Tips for Teamwork

- Use Pull Requests for review.
- Comment on each other's work.
- Try assigning tasks like: "Add animations", "Improve layout", etc.

---

## ✅ Sample `index.html` Setup

```html
<div class="cards">
  <iframe src="members/alice.html"></iframe>
  <iframe src="members/bob.html"></iframe>
</div>
```

---

## 📸 Screenshots

_Add screenshots here of your awesome cards in action_

---

Happy coding! 🚀