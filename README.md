# mtm6201-final
# Plant Palette — Final Project

## Overview
This website was created as part of my final assignment for Web Development. It represents a three page restaurant website built with HTML, CSS, Bootstrap, and a small amount of JavaScript. The site includes a custom designed navbar, responsive sidebar, fully styled cards, and dynamic layouts that adjust for both desktop and mobile experiences. The goal was to build a professional, responsive, and visually cohesive website while maintaining strict consistency across all pages.

---

## My Process
When I started this project, I focused on building a clean foundation that could be reused across all pages. I created a global structure containing:

- A reusable navbar
- A reusable sidebar that collapses on mobile
- A reusable footer
- A single unified CSS file that styles everything

Once this structure was stable, I created three different pages:

1. Home – “Our Information” section with three informational cards  
2. Meals – three cards for different menu categories  
3. Reservations – three functional cards related to booking, canceling, and checking reservations  

Each page reuses the same global layout, but the card design changes depending on page purpose.

---

## Challenges I Faced and How I Solved Them

### 1. Creating a Responsive Navbar Without Bootstrap’s Toggler
One of the first challenges was that Bootstrap's default mobile navbar toggler did not match my mockup or behavior requirements. I needed:

- Navbar links centered in mobile view  
- Social icons aligned to the right  
- A custom hamburger button outside the navbar  

To solve this:
- I hid Bootstrap’s toggler completely  
- I created my own hamburger button  
- I wrote custom CSS and JavaScript so the sidebar opens only over the <main> area instead of covering the navbar or footer  

This required several layout adjustments, but the final result matched my design perfectly.

---

### 2. Getting the Sidebar to Behave Properly on Mobile
The sidebar was the most challenging part. It had to:

- Slide open  
- Slide closed  
- Stay inside the <main> content  
- Never cover the navbar or footer  
- Close when clicking anywhere outside of it  

I solved this by:
- Positioning the sidebar absolutely inside <main>
- Adding a custom semi-transparent overlay
- Using JavaScript to toggle .sidebar-open and .overlay-active classes

Once everything clicked, it behaved exactly like a professional mobile sidebar.

---

### 3. Mobile Layout for Cards
Each page uses cards, but all behave differently:

- Home page: Cards are vertical on desktop but become horizontal on mobile (text left, image right).
- Meals page: Cards start with the image, then the paragraph, then the button.
- Reservations page: Same structure, but with a different card color and different button behavior.

I had to write responsive CSS using grid and flex to ensure:

- Images align on the right  
- Text aligns on the left  
- Buttons move below the text  
- Images touch the top and bottom edges on mobile  
- Desktop and mobile styles never overwrite each other  

This was one of the trickiest parts of the project, but it taught me a lot about responsive layouts and structuring CSS cleanly.

---

### 4. Ensuring All Images Have Matching Sizes
My mockups required all card images to be the same height and width across the three cards. This meant using:

- aspect-ratio  
- object-fit: cover  
- Responsive wrappers  

This allowed every image to remain equal without stretching or looking distorted.

---

### 5. Managing a Single Global CSS File
With three different pages and multiple card styles, it was difficult to avoid conflicts. I solved this by:

- Using very specific selectors (ex: .meal-card .read-more-btn)  
- Grouping CSS into large labeled sections  
- Making sure mobile queries only apply to their intended elements  
- Keeping Home, Meals, and Reservations modular and separate within the same file  

This taught me how to properly scale CSS for multi-page websites.

---

## What I Learned

- How to build a fully responsive website from scratch  
- How to structure a large CSS file without creating conflicts  
- How to design for both desktop and mobile simultaneously  
- How to use and override Bootstrap effectively  
- How to write custom JavaScript for UI behavior  
- How to debug layout issues (lots of trial and error!)  
- How to match a design mockup with precise spacing, alignment, and color  
- How to organize a multi-page website while keeping everything consistent  

Overall, this project helped me grow significantly in front-end development, responsive design, and code organization.

---

## Assets & Resources Used

### Frameworks / Libraries
- Bootstrap 5.3 (layout, grid, spacing utilities)
- Animate.css (subtle animations)
- ScrollReveal.js (scroll-based text animation)

### Fonts
- Panton Narrow (Regular + ExtraBold) — Dafont  
- Recoleta DEMO — Dafont  

### Icons & Images
- Custom PNG and JPG assets used for:
  - Navbar icons (Instagram + X)
  - Sidebar icons
  - Card images (Home, Meals, Reservations)
  - Footer logo  

All images used were generated by myself or provided for educational use.

### Figma Design
https://www.figma.com/design/i5KAdXc4Wm7rBaf4ZHJqd1/Untitled?node-id=0-1&p=f&t=67uh1FScwFiu6Cmm-0

---

## Final Notes
This project required a lot of debugging, patience, and attention to detail, but I am proud of how it turned out. I learned how to think like a designer and a developer at the same time and how to solve problems creatively without breaking the rest of the website.

Thank you for reviewing my work!
Ayelen Tatiana Ruggirello