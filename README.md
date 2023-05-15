# Social Proof Section Solution - Frontend Mentor

![Design preview for the Social proof section coding challenge](./design/desktop-preview.jpg)

## Welcome! 👋

Hello everyone! 😁

This is my solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA).

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](images/social-proof-section-desktop.png)
![](images/social-proof-section-mobile.png)

### Links

- Solution URL: [Github](https://github.com/daisukeeita/Social-Proof-Component)
- Live Site URL: [Social Proof Section Solution](https://daisukeeita.github.io/Social-Proof-Component/)

## My process

### Built with

<!-- Badges -->

![](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

The application of reponsiveness of the website/section. 

I applied the 'Fluid Typography' in the `font-sizes`, using the `clamp()` function. 

```css
    :root{
        --font-size-testimonial: 1rem;
        --font-size-rating: clamp(17px, calc(1.0625rem + ((1vw - 3.75px) * 0.0939)), 18px);
        --font-size-heading: clamp(39.2px, calc(2.45rem + ((1vw - 3.75px) * 1.3897)), 54px);
        --font-size-subHeading: clamp(17.5px, calc(1.09375rem + ((1vw - 3.75px) * 0.2347)), 20px);
    }
```

I also used the Grid for the layout of the section. Applying the 'fluidity' in Grid takes a lot of time if you're not used to implement it. 

```css
    .social-proof-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(371px, 1fr));
        grid-template-rows: 293px 293px;
        grid-template-areas: 
            '.heading-subHeading-section .rating-section'
            'reviews-section';
        width: 87.47vw;
        max-width: 1112px;
    }
```

Applying this technique is actually hard to implement especially if there's so much to manipulate. But it was satisfying once you finished the implementation.  
