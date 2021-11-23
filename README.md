# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)



## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![finished-desktop-screenshot](images/finished-desktop-screenshot.jpg)

Finished-desktop-screenshot

![mobile-hover-state](images/mobile-hover-state-screnshot.jpg)

Mobile-hover-state

### Links

- Solution URL: [My solution](https://www.frontendmentor.io/solutions/nft-preview-challenge-by-a-newbie-without-flex-and-grid-GDLHiNwsB)
- Live Site URL: [Nft-preview-live-site](https://niraj-kumar-nft-preview.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties


### What I learned

1) I learn't how to vertically center an image inside a div, without flex (I haven't started flexbox or grid as of 23rd Nov 2021, so I wanted to use only plain css, and stuff I already know, to complete this project for now)

```css
.parent{
  position: relative;
}

.child{
  position: absolute;
  /* This sets the top left corner of the image at the centre of the parent element*/
  top: 50%;
  left: 50%;

  /* This sets the translates the image so that its centre aligns with the parent element's cemtre */
  transform: translateX(-50%) translateY(-50%);
}
```

2) I learn't that ::before and ::after pseudo elements don't work, on img tags, as they don't have any text content.


3) I learn't how to use the hover selector to do thing to a class other than te one over which hovering is done.
```css
.image:hover .image-equilibrium-overlay-div{
    opacity: 1;

/* This is saying that when you see that .image class is in the hover state, change the opacity of .image-equilibrium-overlay-div class to 1 */
    
}
```

### Useful resources

- [Why before and after pseudo elements don't work with img tag](https://stackoverflow.com/questions/5843035/does-before-not-work-on-img-elements) - This helped me beacause I was trying to get the hover effect over the image by using an after pseudo element, but as it turns out, it won't work, like at all.

- [How to center an image inside a div, both horizontally,and vertically](https://www.freecodecamp.org/news/how-to-center-an-image-in-css/) - This is an amazing article which helped me to vertically center an image inside a div. I'd recommend it to anyone still learning this concept.


## Author

<!-- - Website - [Add your name here](https://www.your-site.com) -->
- Frontend Mentor - [@niraj-kumar-r](https://www.frontendmentor.io/profile/niraj-kumar-r)
- Twitter - [@niraj_kumar_r](https://twitter.com/niraj_kumar_r)
