# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 


# What I learned

By coding this challenge I learned about different things: 
- Planing my project before starting to code: I took paper and pencil to plan how I was going to organize the projects, how I was going to organice the HTML and CSS, and what were tha challenges that I though I was going to find. 
- Finding documentation: before starting to code I realized that I needed some documentation on different topics that I would need to learn or review. For example, the best practices to center elements, how to add content (a background and an icon) on hover, how to add svg's...
- Organizing my code: I learned that it is very important to organize and comment my code very accurately to be able to understand it and reuse it later. 
- I learned more about CSS functions and specially the var function 

More specifically, I learned how to: 
- Make a hover state like the one in this project with an icon. It was challenging because I had never done it before. 
The HTML to do it looks like this: 

```html
<a href="#">
    <div class="img">
      <img src="images/image-equilibrium.jpg" alt="Equilibrum Corporate Image">
      <div class="img-overlay">
      </div>
      <div class="hover-icon">
        <svg width="48" height="48" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path d="M0 0h48v48H0z"/><path d="M24 9C14 9 5.46 15.22 2 24c3.46 8.78 12 15 22 15 10.01 0 18.54-6.22 22-15-3.46-8.78-11.99-15-22-15Zm0 25c-5.52 0-10-4.48-10-10s4.48-10 10-10 10 4.48 10 10-4.48 10-10 10Zm0-16c-3.31 0-6 2.69-6 6s2.69 6 6 6 6-2.69 6-6-2.69-6-6-6Z" fill="#FFF" fill-rule="nonzero"/></g></svg>
      </div>
    </div>
  </a> 
```

The CSS looks like this: 
```css
/* Main image*/
.img {
  position: relative;
  width: 100%;
}

.img img {
    display: block;
    width: 100%;
    border-radius: 3%;
}

/* --Aligning the icon to the center and not showing it */
.hover-icon {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    text-align: center;
    opacity: 0;
  }

/* --Adding the overlay for the image and not showing it */
.img-overlay {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: .3s ease;
    background-color: var(--cyan);
    border-radius: 3%;
  }

/* --Showing the overlay for the image and icon on hover */
.img:hover .img-overlay {
    opacity: 0.5;
}

.img:hover .hover-icon {
    opacity: 1;
}
```
- How to create a line in HTML and give it style to CSS: 
```html
<hr>
```

```css
hr {
    height: 0px;
    border: none;
    border-top: 0.5px solid var(--line);
}
```

# Continued development

I will like to continue focusing on how to make my projects responsive. I found it easy for this one, but I think it is a very important topic to continue working on it. 

# Useful resources

- [CSS Functions](https://www.w3schools.com/cssref/css_functions.asp) - This helped me understand CSS functions. I wanted to use the var function to easily add the correct colors to CSS. 
- [How TO - Image Overlay Icon](https://www.w3schools.com/howto/howto_css_image_overlay_icon.asp) - This is where I found the information to create the overlay layer with the icon.
- [HTML <hr> Tag](https://www.w3schools.com/tags/tag_hr.asp) - This is where I found more information about the hr tag and how to style it properly.

