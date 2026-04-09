# Issues Found & Fixed — Homework 1

## Issue 1
- **What I Found:** On mobile the navigation menu was taking up too much screen space. For phone users specifically this would make for a not good experience navigating the website.
- **Why It Matters:** For phone users specifically this would make for a not good experience navigating the website.
- **How I Fixed It:** I initially approached this issue by making the menu disappear or reappear when scrolling up or down. This solution felt off and awkward however so I asked for the menu display to be horizontal like on desktop or tablet and updated the background color for the menu

- **Before:** 
```css
@media (max-width: 480px) {
  nav ul {
    gap: 0.5rem;
    flex-direction: column;  /* Vertical stacking */
  }
}
```
```css
nav {
  background-color: #fff;  /* White background */
}
```
- **After:** 
```css
@media (max-width: 480px) {
  nav ul {
    gap: 0.5rem;
    /* Removed flex-direction: column */
  }
}
```
```css
nav {
  background-color: #e8e8e8;  /* Grey background */
}
```

## Issue 2
- **What I Found:** Clicking "View Project" would jump the user to the top of the page.
- **Why It Matters:** This felt awkward and confusing because users expected project details, not a page jump.
- **How I Fixed It:** I decided to implement a pop up window that would display information for that specific project. 
```html
<a href="#" class="project-card-link">View Project</a>
```
- **After:**
```html
<button class="project-card-link" data-project="0">View Project</button>
```
```javascript
document.querySelectorAll('.project-card-link').forEach((button) => {
  button.addEventListener('click', (e) => {
    e.preventDefault();
    const projectId = button.getAttribute('data-project');
    openProjectModal(projectId);
  });
});
```

## Issue 3
- **What I Found:** After implementing the popup, clicking "View Project" still did not open the modal.
- **Why It Matters:** This broke the intended project interaction and made the button appear non-functional.
- **How I Fixed It:** There were parsing issues in portfolia.html, removing the javascript block that was misplaced and putting in the write section fixed this issue.

- **Before:**
```html
<style>
  ...
  <script>
    // PROJECT MODAL FUNCTIONALITY (misplaced)
  </script>
  body {
```
```javascript
// Modal handlers were not running correctly from the intended script block
```
- **After:**
```html
<style>
  ...
  body {
```
```javascript
function openProjectModal(projectId) {
  const project = projectData[projectId];
  const modal = document.getElementById('projectModal');
  modal.classList.add('show');
}
```

