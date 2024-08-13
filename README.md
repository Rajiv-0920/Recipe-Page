# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). 

## Table of contents

- [Frontend Mentor - Recipe page solution](#frontend-mentor---recipe-page-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
  - [Author](#author)

## Overview

The "Recipe Page Solution" from Frontend Mentor features a clean layout with a recipe image, preparation details, ingredients list, instructions, and nutritional info, offering a user-friendly and visually appealing cooking experience.

### Screenshot

![Recipe Page Solution Screenshot](./solution/Recipe%20Page%20Solution.png)

### Links

- Solution URL: [Recipe Page Repo](https://github.com/Rajiv-0920/Recipe%20Page/)
- Live Site URL: [Recipe Page Solution](https://rajiv-0920.github.io/Recipe%20Page/)

## My process

During the development phase, I used HTML and CSS to create the interactive elements. One challenge I encountered was ensuring the layout remained responsive across different devices, which I addressed by employing a mobile-first design approach and conducting extensive testing.

### Built with

- HTML5 - For the structure and content of the page.
- CSS3 - For styling, layout, and responsive design.
- Frontend Mentor - As the platform for the challenge and design inspiration.
- VS Code - As the code editor.
- GitHub - For hosting the code repository.

### What I learned

**CSS Custom Properties (Variables):**

Code Example:

```css
:root {
    --White: hsl(0, 0%, 100%);
    --Stone100: hsl(30, 54%, 90%);
    --Stone150: hsl(30, 18%, 87%);
    --Stone600: hsl(30, 10%, 34%);
    --Stone900: hsl(24, 5%, 18%);
    --Brown800: hsl(14, 45%, 36%);
    --Rose800: hsl(332, 51%, 32%);
    --Rose50: hsl(330, 100%, 98%);
}
```

Learning: Defined variables for colors, font families, font sizes, and other properties to ensure consistency and simplify updates.

**Font Loading with @font-face:**

Code Example:

```css
@font-face {
    font-family: 'Outfit';
    src: url('./assets/fonts/outfit/static/Outfit-Regular.ttf');
}

@font-face {
    font-family: 'Young Serif';
    src: url('./assets/fonts/young-serif/YoungSerif-Regular.ttf');
}
```

Learning: Loaded custom fonts into the stylesheet using @font-face, ensuring specific fonts are used.

**CSS Reset and Base Styles:**

Code Example:

```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: var(--Outfit);
    font-size: var(--font-size-base);
    font-weight: var(--font-weight-normal);
    color: var(--Stone600);
}
```

Learning: Applied a CSS reset to ensure consistent styling across browsers and set base styles for the body and common elements.

**Responsive Design:**

Code Example:

```css
@media (min-width: 43.75em) {
    main {
        background-color: var(--Stone100);
    }
    .recipe-details {
        width: min(75vw, 700px);
        margin: calc(var(--spacing-unit) * 10) 0;
        border-radius: calc(var(--border-radius) * 2);
    }
}
```

Learning: Used media queries to adjust styles for different screen sizes, ensuring a responsive design.

**Dynamic Values with calc() and clamp():**

Code Example:
```css
.recipe-title {
    font-size: calc(var(--font-size-base) * 2.3);
}

.recipe-img {
    margin: clamp(25px, calc(3.5vw + 2px), calc(var(--spacing-unit) * 3.5)) auto;
}
```

Learning: Used calc() for calculations and clamp() for responsive values that adjust within a defined range.

### Continued development

**Advanced Responsive Design:**

Concepts to Explore: Responsive design techniques beyond media queries, such as container queries and fluid typography.

Goals: Refine skills in making designs adapt fluidly to various screen sizes and orientations, and implement modern responsive features for more dynamic layouts.

**CSS Grid and Flexbox:**

Concepts to Explore: Advanced CSS Grid and Flexbox layouts, including nested grids, alignment techniques, and complex layouts.

Goals: Perfect the use of Grid and Flexbox for creating intricate and flexible layouts. Experiment with combining both for more powerful layout solutions.

**Performance Optimization:**

Concepts to Explore: Techniques for optimizing CSS performance, such as minimizing CSS file size, avoiding excessive use of calc() and clamp(), and managing complex selectors.

Goals: Ensure that CSS remains performant and efficient, particularly in large projects with complex styles.

## Author

- Website - [Rajiv Kumar](https://rajiv-0920.github.io/Portfolio/)
- Frontend Mentor - [@Rajiv-0920](https://www.frontendmentor.io/profile/Rajiv-0920)
- Twitter - [@Rajiv_0920](https://www.twitter.com/Rajiv_0920)
