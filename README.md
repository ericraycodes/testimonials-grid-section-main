# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)



## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size


### Links

- Solution URL: [https://github.com/ericraycodes/four-card-feature-section-master](https://github.com/ericraycodes/four-card-feature-section-master)
- Live Site URL: [https://ericraycodes.github.io/four-card-feature-section-master](https://ericraycodes.github.io/four-card-feature-section-master)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

I learned more on **CSS Grid**. It was good to learn how it can work well with **Flexbox**.

```css
.card-grid {
  /* arrange content */
  padding: 2em;
  display: grid;
  grid-template-rows: repeat(2, 1fr);
  grid-template-columns: repeat(3, 1fr);
  row-gap: 2em;
}
.card-header {
  grid-area: 1/1/2/4;
  place-self: start start;

  /* arrange content */
  display: flex;
  flex-direction: column;
  gap: 0.25em;
}
.card-icon {
  grid-area: 2/3/3/4;
  place-self: center end;
}
```
```css
.cards-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-areas:
      "supervisor team-builder calculator"
      "supervisor karma calculator";
    align-items: center;
  }
  .supervisor {
    grid-area: supervisor;
  }
  .team-builder {
    grid-area: team-builder;
  }
  .karma {
    grid-area: karma;
  }
  .calculator {
    grid-area: calculator;
  }
```

I discovered that a **negative** *spread radius* on *box-shadows* can make the shadows look neat - my perspective, depending on visual use.

```css
  box-shadow: 0 0.67em 1.25em -0.25em var(--shadow-color);
```


### Continued development

- Continuing to work on _Mobile-first Design_.

## Author

- Frontend Mentor - [@ericraycodes](https://www.frontendmentor.io/profile/ericraycodes)
- GitHub - [ericraycodes](https://github.com/ericraycodes)
