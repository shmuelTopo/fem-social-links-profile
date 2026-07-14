# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ).

## Overview

A responsive profile card that displays a user's profile information and social media links. The design features a dark theme with a lime-green accent color and smooth hover interactions on all link elements.

## Features

- ✨ Responsive card layout centered on all screen sizes
- 🎨 Dark theme with custom color variables
- 🔗 Interactive social media links with hover effects
- 📱 Mobile-first responsive design using `clamp()`
- ♿ Semantic HTML structure
- 🎯 Smooth visual feedback on interaction

## Built with

- **HTML5** - Semantic markup with `<article>`, `<ul>`, and `<li>` elements
- **CSS3** - Custom properties (CSS variables) for maintainable theming
- **Flexbox** - For layout alignment and spacing
- **Responsive Design** - Using `clamp()` for fluid sizing
- **Custom Font** - Inter font loaded locally from assets

## Technical highlights

**CSS Variables for Theme Management:**
```css
:root {
  --color-green: #c4f82a;
  --color-grey-700: #333333;
  --color-grey-800: #1f1f1f;
  --color-grey-900: #141414;
  --color-white: #ffffff;
  --spacing-300: 24px;
  /* ... more variables */
}
```

**Responsive Card Width:**
```css
article {
  width: clamp(100%, 384px, calc(100vw - 2rem));
}
```
This ensures the card stays fluid on small screens, reaches a max of 384px, and respects viewport margins.

**Flexbox Centering:**
- Used `flex-direction: column` to stack elements vertically
- Combined `justify-content` and `align-items` to center content
- Set `gap` property for consistent spacing between elements

**Interactive Hover States:**
```css
li:hover {
  background-color: var(--color-green);
  color: var(--color-grey-700);
  opacity: 0.8;
  cursor: pointer;
}
```

## Layout structure

```
Body (flex container, full height)
  └── Main (flex, centered)
      └── Article (card)
          ├── Avatar (circular image)
          ├── General info (name + location)
          ├── Occupation (quote)
          └── Social links (list)
```

## Author

Built by Shmuel Toporowitch
- Frontend Mentor - [@Shmuel](https://www.frontendmentor.io/profile/Shmuel)
