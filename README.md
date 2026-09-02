# Personal Portfolio Website

## Overview

This project is my first major project completed as part of a Full Stack Web Development Bootcamp.

For the project, we were given the choice of creating either a **personal portfolio website** or a **hobby website**. I chose to build a personal portfolio because it gave me an opportunity not only to consolidate the HTML and CSS skills I had learned so far, but also to explore areas of front-end development that I wanted to improve.

My main objective was to use the project as a learning opportunity. Rather than simply meeting the minimum project requirements, I wanted to challenge myself to create a website that felt polished, professional and personal.

In particular, I wanted to improve my understanding of:

- CSS animations and transitions
- Micro-interactions
- Scroll-driven animations
- Responsive design
- Flexbox layouts
- Typography and visual hierarchy
- Accessibility
- SVG graphics
- Wireframing and planning
- Creating a more premium and professional-looking user interface

---

## Project Goals

The primary goal of the project was to create a responsive personal portfolio website that could showcase my skills, experience and development projects.

From a learning perspective, I wanted to move beyond simply building functional page layouts and focus more closely on the details that contribute to the overall user experience.

I therefore focused on creating:

- A clean and modern visual design
- Clear content hierarchy
- Consistent navigation
- Responsive layouts across different screen sizes
- Subtle animations and interactions
- A strong typography system
- A portfolio that reflects some of my personality rather than feeling like a generic template

---

## Planning and Design

One of the most important lessons I wanted to apply during this project was the importance of planning before beginning development.

Instead of immediately writing HTML and CSS, I first created a **wireframe** for the website. This helped me think about the structure of each page and section before implementing the design.

The wireframes can be viewed in the project repository:

> **Wireframes:** [Add link to wireframes here]

I also researched existing developer portfolio websites to better understand how professional portfolios present information and use typography, spacing, animation and visual hierarchy.

One portfolio in particular became a major source of design inspiration. I liked its polished and professional appearance and used aspects of its visual direction as inspiration for my own project.

My aim was not to reproduce the website directly, but to understand what made the design effective and adapt those ideas into something that represented my own style.

> **Design inspiration:** [https://refined.framer.website]

---

## Features

### Responsive Navigation

The website includes consistent navigation throughout the site and has been designed to remain usable across desktop, tablet and mobile screen sizes.

Multiple CSS media-query breakpoints are used to adapt the layout and typography depending on the available viewport width.

---

### Technology Carousel

One of the more challenging elements of the project was creating an infinitely scrolling carousel displaying technologies that I have worked with or have some experience using.

The carousel appears as part of the call-to-action area on the homepage and continuously displays technology logos.

Creating this component helped me improve my understanding of:

- CSS keyframe animations
- Overflow handling
- Flexbox
- Animation timing
- Repeating animation loops
- SVG assets

---

### Scroll-Driven Animations

I experimented with modern CSS scroll-driven animation features to animate elements as they enter the viewport.

For example:

```css
.autoShow {
    animation: text-appear linear both;
    animation-timeline: view();
    animation-range: entry 20% cover;
}
```

This was particularly interesting because modern CSS can now achieve some effects that would previously have required JavaScript or a dedicated animation library.

Working with these properties gave me a better understanding of the direction modern CSS is moving in and how browser-native animation APIs can be used to create richer interfaces.

---

### Micro-Interactions and Transitions

A major personal learning goal for this project was improving my understanding of CSS transitions and animations.

I experimented with subtle motion throughout the site to make interactions feel more deliberate and polished without overwhelming the user.

This included learning more about when animation is appropriate, how animation timing affects the user experience, and how motion can be used to reinforce visual hierarchy.

---

## Accessibility

Accessibility was considered throughout the development process.

Images include appropriate alternative text where required, and I also researched the accessibility implications of animation.

In particular, I learned about the importance of respecting users who prefer reduced motion through the `prefers-reduced-motion` media query.

For example:

```css
@media (prefers-reduced-motion: reduce) {
    /* Reduce or disable non-essential animations */
}
```

This was an important reminder that animations should enhance an interface rather than make a website more difficult to use.

---

## Typography

Typography plays a significant part in the visual identity of the website.

I used three typefaces, each with a specific purpose:

- One typeface for the personal logo/name
- One typeface for headings and titles
- One typeface for body content

The fonts were imported using **Google Fonts**.

Careful attention was also given to:

- Font size
- Font weight
- Line height
- Spacing
- Heading hierarchy
- Responsive typography

The aim was to create a clear visual hierarchy while maintaining a consistent design language throughout the site.

---

## SVG Assets

SVG graphics are used extensively throughout the project, particularly for technology logos and icons.

Using SVG files allowed the graphics to remain sharp at different screen resolutions while also keeping them suitable for responsive layouts.

Working with SVGs also gave me more experience with how externally sourced graphical assets interact with HTML, CSS and validation tools.

---

## Technologies Used

The project was primarily built using:

- HTML5
- CSS3
- Flexbox
- CSS Grid where appropriate
- CSS Media Queries
- CSS Animations
- CSS Transitions
- CSS Scroll-Driven Animations
- Google Fonts
- SVG graphics
- Git
- GitHub

---

## HTML Structure

The site uses semantic HTML wherever appropriate.

Elements used throughout the project include:

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

The project also includes:

- A correctly structured HTML document
- `<head>` and `<body>` elements
- Page titles
- Viewport metadata
- External CSS stylesheets
- Semantic page sections
- Accessible image alternative text
- Consistent navigation

---

## Responsive Design

The website was designed using a responsive approach.

I used a combination of:

- Flexbox
- Flexible sizing
- Responsive typography
- Relative units
- Media queries
- Multiple layout breakpoints

This allowed the website to adapt to a range of desktop, tablet and mobile screen sizes.

Working on the responsive behaviour of the site significantly improved my understanding of media queries and how layouts need to change rather than simply shrink as the viewport becomes smaller.

---

## CSS Frameworks

One of the suggested project requirements was the use of a CSS framework such as **Bootstrap** or **Tailwind CSS**.

I ultimately decided not to use a CSS framework for this project.

The visual design I was trying to achieve required a relatively custom interface, and I felt that writing the layout and styling myself would provide a better learning experience.

Instead, I relied heavily on:

- Custom CSS
- Flexbox
- Responsive media queries
- Modern CSS selectors
- SVG assets

Although this meant that I did not fulfil the CSS framework portion of the original brief, it allowed me to spend more time developing my understanding of CSS itself.

---

## Advanced CSS

Throughout the project I experimented with several modern CSS techniques and selectors.

These included selectors and features such as:

```css
:nth-child()
:has()
:where()
```

I also explored newer CSS animation properties and viewport-driven effects.

This gave me a much better understanding of what can now be achieved using native CSS without relying immediately on JavaScript.

---

## CSS Custom Properties

I did not make significant use of CSS custom properties (`--variables`) in this version of the project.

During development, however, I learned more about how useful they are for maintaining values such as:

- Colours
- Spacing
- Font sizes
- Reusable design tokens
- Animation settings

This is something I intend to make greater use of in future projects and would be one of the areas I would refactor if I returned to this project.

---

## Validation

### HTML Validation

The project was tested using the W3C HTML Validator.

Some validation warnings/errors were encountered in relation to SVG markup.

When I attempted to remove some of the SVG attributes identified by the validator, doing so caused the affected graphics to stop working correctly. Because these SVG files originated from external assets, I retained the required markup where removing it would break the intended rendering.

This highlighted an important distinction between blindly removing every validator warning and understanding why a particular piece of markup exists.

---

### CSS Validation

The stylesheet was also checked using the W3C CSS Validator.

The validator reports errors for some of the modern scroll-driven animation properties used in the project, including:

```css
animation-timeline: view();
animation-range: entry 20% cover;
```

For example, the validator may report:

```text
Property animation-timeline doesn't exist
Property animation-range doesn't exist
```

These properties are part of the newer **CSS Scroll-Driven Animations** specification and may not be recognised when the validator is checking against an older CSS profile such as CSS Level 3.

The declarations are intentionally used as part of the project's experimentation with modern CSS.

---

## Challenges

### Learning CSS Animation

One of the biggest challenges during this project was developing a better understanding of CSS animation.

Before starting the project, animations and transitions were an area in which I had relatively little confidence.

Through building the website, I gained practical experience with:

- `@keyframes`
- `animation`
- `transition`
- Animation timing functions
- Infinite animation loops
- Scroll-driven animation
- View timelines
- Reduced-motion accessibility

This was one of the most valuable areas of learning during the project.

---

### Infinite Technology Carousel

The technology carousel was one of the more technically challenging components.

I wanted the logos to continuously move through the interface in a seamless loop without an obvious beginning or end.

Getting the spacing, animation timing and repetition correct required experimentation, but the process helped reinforce my understanding of how CSS animations and layout systems work together.

---

### Achieving a Professional Visual Design

Another challenge was moving from a technically functional website to one that felt visually polished.

I spent considerable time adjusting details such as:

- Typography
- Spacing
- Alignment
- Animation timing
- Font weights
- Responsive behaviour
- Section hierarchy
- Visual consistency

This reinforced how much attention to detail contributes to the perceived quality of a website.

---

## Testing

During development, I tested the website across multiple viewport sizes using browser developer tools.

Testing focused on:

- Navigation
- Responsive layouts
- Typography
- Image scaling
- SVG rendering
- Animation behaviour
- Scroll-triggered effects
- Content readability
- Overflow issues

The site was also reviewed using W3C validation tools for both HTML and CSS.

---

## What I Learned

This project helped consolidate much of what I had learned about HTML and CSS during the course while also encouraging me to explore more advanced techniques independently.

The most valuable areas of learning were:

- Planning a website using wireframes
- Translating a design into HTML and CSS
- Building responsive layouts
- Using Flexbox more confidently
- Working with SVG graphics
- Creating CSS animations
- Creating infinite animation loops
- Using modern scroll-driven CSS
- Understanding reduced-motion accessibility
- Working with multiple typography styles
- Improving visual hierarchy
- Using modern CSS selectors
- Understanding the limitations of automated validators

Most importantly, the project showed me the value of using projects not only to demonstrate what I already know, but also to deliberately explore areas where my knowledge is weaker.

---

## Future Improvements

If I continue developing the project, some areas I would like to improve include:

- Refactoring repeated values into CSS custom properties
- Further improving accessibility
- Testing across a wider range of browsers and physical devices
- Adding fallbacks for newer CSS animation features
- Optimising SVG and other static assets
- Continuing to refine animation performance
- Improving project content as I complete additional projects
- Reviewing opportunities to simplify and refactor the CSS

---

## Credits

### Fonts

Fonts used throughout the project were sourced from:

- [Google Fonts](https://fonts.google.com/)

### Icons and SVGs

Technology icons and SVG assets were sourced from:

> [Add SVG library/resource name and link here]

### Design Inspiration

The visual direction of this portfolio was inspired in part by:

> [Add original portfolio / Framer inspiration link here]

The final website was designed and developed independently for this project.

---

## Project Reflection

My main goal with this project was to learn as much as possible rather than restrict myself only to techniques already covered during the course.

The project pushed me to research modern CSS, animation, accessibility and interface design in greater depth.

There were several points where I had to experiment, make mistakes and rethink my approach, particularly when working with animation and responsive layouts. That process ultimately made the project much more valuable as a learning experience.

I now feel much more confident working with CSS animations, responsive design and modern CSS features, and I plan to carry what I learned here into future projects.
