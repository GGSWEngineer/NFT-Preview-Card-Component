# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements


### Links

- Solution URL: https://github.com/GGSWEngineer/NFT-Preview-Card-Component
- Live Site URL: https://ggswengineer.github.io/NFT-Preview-Card-Component/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
 <div class="product">
            <img class="product_img" src="./images/image-equilibrium.jpg" alt="equilibrium cube">
            <img class="product_img_active" src="./images/icon-view.svg" alt="eye icon in the middle of the cube with cyan background color">
          </div>
```
```css
.product {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 24px;
}

.product_img {
  width: 278px;
  height: 278px;
  border-radius: 8px;
}

.product_img_active {
  width: 278px;
  height: 278px;
  position: absolute;
  background-color: hsla(178, 100%, 50%, 0.5);
  padding: 108px;
  border-radius: 8px;
  display: none;
}

.product:hover {
  cursor: pointer;
}

.product:active .product_img_active {
  display: block;
}
```
This html / css pattern can be used to change the complexion of an already existing image by using an image that doesn't display until it is active. 

Using position: absolute, the image is positioned to the top left corner of its nearest ancestor which in this case is the .product container. I like to think that the image is hiding until it is activated once it is clicked on adding that cyan complexion to the original image. 

// 

When using display: flex, or display: grid,  gap is an essential property to give space between the grids rows and columns instead of using box model properties like margin, or padding. 

//

Bootstraps media queries are an awesome place to get sizes to make the webpage responsive. This one is a small project but I used their min-width: 992px for desktops and it worked great. Will be using this a lot moving forward. 


## Author

- Frontend Mentor - [@GGSWEngineer](https://www.frontendmentor.io/profile/GGSWEngineer)
- LinkedIn - [Gerardo Garcia](www.linkedin.com/in/gerardo-garcia-19a794275)


## Acknowledgments

Thanks so much to @Better5afe on frontendmentor.io for helping out by posting a comment on my last solution. Her advice helped out with this project!
