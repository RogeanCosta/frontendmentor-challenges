# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### Screenshot

**Result for Desktop Design**

![](./design/stats-preview-card-component-desktop-solution.PNG)

**Result for mobile Design** </br>

![](./design/stats-preview-card-component-mobile-solution.PNG)

### Links

- Solution URL: https://github.com/RogeanCosta/frontendmentor-challenges/tree/main/stats-preview-card-component
- Live Site URL: https://rogeancosta.github.io/frontendmentor-challenges/stats-preview-card-component/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

How to add color overlay to an image:

```css
.card-img-container {
  width: 33.75rem;
  height: 27.875rem;
  position: relative;
}

.card-img-container::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: var(--soft-violet);
}

.card-img {
  display: block;
  max-height: 100%;
  mix-blend-mode: multiply;
  opacity: 0.7511;
}
```

</br>How to define in HTML which image will be loaded based on the screen size:

```html
<picture>
  <source
    class="card-img"
    media="(max-width:1000px)"
    srcset="./images/image-header-mobile.jpg"
  />
  <img
    class="card-img"
    src="./images/image-header-desktop.jpg"
    alt="a group of three women working on their notebooks."
  />
</picture>
```

### Continued development

I would like to continue learning new and interesting things such as the blend mode applied to the photo. I would also like to continue improving my knowledge about Flexbox.

### Useful resources

- [Discussion on hubspot](https://community.hubspot.com/t5/CMS-Development/Adding-a-colour-overlay-to-an-image/m-p/780238#:~:text=To%20add%20a%20color%20overlay,a%20semi%2Dtransparent%20background%20color.&text=In%20this%20code%2C%20the%20%3A%3A,to%20cover%20the%20entire%20area.) - This feature helped me in the process of adding a color layer to the grayscale image.
- [Multiples Images](https://www.w3schools.com/tags/tag_picture.asp) -
  This page helped me in the process of defining which image will be loaded in the HTML depending on the screen size.

## Author

- Frontend Mentor - [@RogeanCosta](https://www.frontendmentor.io/profile/RogeanCosta)
- Linkedin - [@Rogean C.](https://www.linkedin.com/in/rogean-c-884a01b8)
