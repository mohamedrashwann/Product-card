# Frontend Mentor - Product Preview Card Component Solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

---

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size (responsive design).
- See hover and focus states for interactive elements.

### Screenshot

![Screenshot of the Product Preview Card Component solution](https://private-us-east-1.manuscdn.com/sessionFile/ZtI8jjy0vpJlY3eLeVJ2hW/sandbox/AOCkauJK699zVFDm2cTQCo-images_1764534333104_na1fn_L2hvbWUvdWJ1bnR1L3NjcmVlbnNob3Q.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvWnRJOGpqeTB2cEpsWTNlTGVWSjJoVy9zYW5kYm94L0FPQ2thdUpLNjk5elZGRG0yY1RRQ28taW1hZ2VzXzE3NjQ1MzQzMzMxMDRfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwzTmpjbVZsYm5Ob2IzUS5wbmciLCJDb25kaXRpb24iOnsiRGF0ZUxlc3NUaGFuIjp7IkFXUzpFcG9jaFRpbWUiOjE3OTg3NjE2MDB9fX1dfQ__&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=iRyTvmbTgPmFaIClKBLGwG~joKutErXegvSaOLNMGzj9EvOKdcWI4tZexBJ5ulFOx2qhGV11QnLcTSRjAL5yujyV-Ca9TWnhpQY69RSJcqA18qmoGBY3F-IQTqeKq0RRse967tDtv7sk1Av4tQLXI4PnrPhBYUAVMJctIL5ISE1uhI8scSRsMezekrABh7W8xFslwNNFPF~KuP5Qgu-gkf4caLZbTqNAbASmnFLslMR5UNBrcmqHraREjR3djnnMUkuk2ELcjObAAI9rifmO6c2WjFLPhENCSPT1qOt8K1tw8ZIyXS2AkE5DA6MEwu6-MmvzQWp6UegXyNRzy9AJQw__)



### Links

- Solution URL (GitHub Repository): [https://github.com/mohamedrashwann/Product-card.git](https://github.com/mohamedrashwann/Product-card.git)
- Live Site URL: [(https://mohamedrashwann.github.io/Product-card/)]

---

## My process

### Built with

This solution was built using the following technologies:

- Semantic **HTML5** markup.
- **CSS Custom Properties** for using the colors defined in the style guide.
- **Flexbox** for component layout and arrangement, including vertical and horizontal centering of the card.
- **Mobile-first** workflow to ensure optimal responsiveness across all devices.

### What I learned

This challenge was an excellent opportunity to reinforce responsiveness skills and handle background images in CSS. Key points of focus included:

1.  **Controlling Layout with Flexbox:**
    Flexbox was used to change the main card's direction from horizontal (row) on desktop screens to vertical (column) on mobile screens using media queries.

    ```css
    /* Default Desktop Layout */
    .card {
      display: flex;
      flex-direction: row; /* Image and text side-by-side */
      /* ... */
    }

    /* Mobile Layout */
    @media (max-width: 600px) {
      .card {
        flex-direction: column; /* Image above text */
      }
    }
    ```

2.  **Responsive Background Images:**
    To ensure the correct image is displayed for each device, the `background-image` CSS property was used with media queries to switch the image between the desktop and mobile versions.

    ```css
    /* Desktop Image */
    .card-img {
      background: url("./image-product-desktop.jpg") center/cover no-repeat;
      width: 50%;
    }

    /* Switch to Mobile Image and set a fixed height */
    @media (max-width: 600px) {
      .card-img {
        background: url("./image-product-mobile.jpg") center/cover no-repeat;
        width: 100%;
        height: 300px; /* Fixed height for mobile image */
      }
    }
    ```

3.  **Implementing Hover States:**
    A hover state was applied to the "Add to Cart" button to change the background color, providing visual feedback to the user.

    ```css
    .btn {
      background: hsl(158, 36%, 37%); /* Primary Green Color */
      /* ... */
    }

    .btn:hover {
      background: hsl(158, 36%, 25%); /* Darker color on hover */
    }
    ```

### Continued development

In future projects, I plan to focus on the following areas:

- **CSS Grid:** Exploring the use of CSS Grid as an alternative to Flexbox for two-dimensional layouts.
- **BEM Methodology:** Applying the BEM (Block, Element, Modifier) methodology to organize class names and make CSS more maintainable.
- **Accessibility:** Further improving accessibility, especially concerning links and focus states, to ensure a better user experience.

### Useful resources

- [Frontend Mentor](https://www.frontendmentor.io/) - The challenge source that helped refine coding skills.
- [Google Fonts - Montserrat](https://fonts.google.com/specimen/Montserrat) - The primary font used in the project.
- [Google Fonts - Fraunces](https://fonts.google.com/specimen/Fraunces) - The font used for headings and prices.

---

## Author

- Name: **Mohamed Rashwann**
- Frontend Mentor: [@mohamedrashwann](https://www.frontendmentor.io/profile/mohamedrashwann)
- GitHub: [@mohamedrashwann](https://github.com/mohamedrashwann)

---

## Acknowledgments

I would like to thank the Frontend Mentor platform for providing this excellent challenge, which helped in applying and improving my CSS and HTML skills.
