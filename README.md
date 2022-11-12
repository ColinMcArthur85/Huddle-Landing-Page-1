# Frontend Mentor - Huddle landing page with a single introductory section

This is a solution to the [Huddle landing page with a single introductory section](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](/src/images/Huddle%20Landing%20Page.png)

### Links

- Solution URL: [Add solution URL here](https://colinmcarthur85.github.io/stats-preview-card-component/)
- Live Site URL: [Add live site URL here](https://colinmcarthur85.github.io/stats-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- SASS
- Custom Properies
- Mixins
- Nesting
- Partials
- SVG

### What I learned

SASS makes like MUCH easier. The nesting ALONE is worth the effort to learn it. I also decided to spend some time trying to understand SVG and the best practices for applying them to a project. What I learned, embeding inline offers more customization, but messy looking HTML (but who cares about that really). Also better for loading as no HTTP requests are required (should probably look into learning more about what this means).

```scss
//Played around with creating reusable classes a-la mixins

.flex-col {
  @include FlexCenter(column, center);
}

.flex-row {
  @include FlexCenter(row, center);
}
```

```scss
//Got nesting down well. Id like to play around with interpolation next project to see if I can but back on how much code Im writting.

.hero {
  &-content {
    text-align: center;
    padding: 3rem;
    & > * {
      color: white;
    }
    &__title {
      font-weight: 700;
      font-size: 2rem;
      padding-bottom: 2rem;
    }
    &__body {
      font-family: $ff-sans;
      font-size: 1.5rem;
    }
    &__button {
      padding: 1rem 7rem;
      border-radius: 2rem;
      margin-bottom: 5rem;
      &:hover {
        background-color: $clr-primary-100;
      }
    }
  }
}
```

### Continued development

I mentioned above. Id like to use tools like interpolation to see if I can minimize the code that I write. Also id like to see if elements like functions have a place for these smaller projects. SASS has been super helpful to learn but Im feeling like its meant for 'bigger things' and these smaller projects are essentially the same thing, which is a good thing as it will just reinforce the basics.

Anyways, looking forward to starting a new project.
