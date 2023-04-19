# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [project duration](#project-duration)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### Screenshot

![the solution screenshot for desktop](/screenshot-desktop.jpg)
![the solution screenshot for mobile](/screenshot-mobile.jpg)


### Links

here is [the link](https://product-preview-card-virid.vercel.app) to the project


## My process

I am a French beginner developer, I started learning HTML and CSS not long ago. 
This is my third project on Frontend Mentor, and this time I also tried to do it without using photoshop to take the dimensions.   
I tried to do the html without by myself, even if I changed the structure of it so many times. 

For this project I found someone on youtube who was doing it, so I watched the video then tried to do it myself a few days later.  
surprisingly, I managed to do the css without any problems. the only small problem I encountered was that my project was growing in size 
because I used units like REM, but I managed to fix that by setting up a media queries. 


### project duration 

Project start : 30 March 2023
End of project : 13 April 2023


### Built with

- Semantic HTML5 markup
- CSS basic properties



### What I learned
I learned that there are other units than px. 
Now I use Rem for text and parts that should be proportional to the font size, for example margins/paddings and font size. 
I put as many properties as possible in my :root so that I can change something that affects the whole site.  

My :root 
```css
:root {
  --clr-primary : hsl(158, 36%, 37%);
  --clr-secondary: hsl(30, 38%, 92%);

  --clr-neutral-500: hsl(212, 21%, 14%);
  --clr-neutral-400: hsl(228, 12%, 48%);
  --clr-neutral-100: hsl(0, 0%, 100%);

  --fs-400: 0,875rem;
  --ff-primary: 'Fraunces', serif;
  --ff-secondary: 'Montserrat', sans-serif;

  --fw-regular: 500;
  --fw-bold: 700;
}
```
exemple of use 
```css
body {
  background: var(--clr-secondary);
  font-family: var(--ff-secondary);
  font-weight: var(--fw-regular);
  font-size: var(--fs-400);
  color: var(--clr-neutral-400);

  display: grid;
  place-content: center;
}
```
I also discovered the "picture" tag, which allows to collect several pictures and to use the most adapted to the user. For example, in this project, I used it so that from a certain screen size, it is another image that is used.  
```html
 <picture class="product__img">
    <source srcset="images\image-product-desktop.jpg" media="(min-width: 650px)">
    <img src="images/image-product-mobile.jpg" alt="product image for mobile">
</picture>
```



## Author

- Frontend Mentor - [@Sid-Shinseo](https://www.frontendmentor.io/profile/sid-shinseo)
