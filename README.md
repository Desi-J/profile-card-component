# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


### The challenge

- Build out the project to the designs provided

### Screenshot

![]("./images/screenshot.png")

### Links

- Solution URL: [here](https://www.frontendmentor.io/solutions/profile-card-component-html-css-BkGegSQBq)
- Live Site URL: [here](https://desi-j.github.io/profile-card-component/)

## My process
  For the middle section (name, age, & location) I used a wrapper div to wrap the content. I gave it a positon of relative so I can push it up moving the image between the wavy card background and the middle section. I tried only giving the image a positon of relative and pushing that up by itself but I had trouble with the margins of the rest of the content not lining up how I wanted. Below is a screenshot, the red border is the wrapper div while the blue border is the middle section. You can see how the wrapper div (red) is being pushed up out of its container (blue).

![]("./images/borders.png")

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned
1. Use relative paths to get images to show up. The "./" is imporitant
   Example:  "./images/example.jpg"

2. transfrom: translate(X,Y);
   The transfrom translate property moves an element (whose position is not static ) from its current position based on the distance you put for the x-axis and y-axis. The element will NOT move out of its place on a screen resize 😀. (Which is exactly what I needed for the background)
 

```html
    <!-- SECTION WITH PHOTO, NAME, & LOCATION -->
    <section class="name">

      <div class="wrapper">
        <img src="./images/image-victor.jpg" alt="Victor Crest">
      <h1>Victor Crest<span>26</span></h1>
      <p class="location">London</p>
      </div>
  
    </section>
```
```css
    /* BACKGROUND CIRCLE IMAGES */
    .circle {
      display: block;
      position: absolute;
      pointer-events: none;
      z-index: 1;
    }

    .top {
      transform: translate(-50%, -40%);
    }

    .bottom {
      transform: translate(45%, 55%);
    }

```

## Author

- Frontend Mentor - [@Desi-J](https://www.frontendmentor.io/profile/Desi-J)

