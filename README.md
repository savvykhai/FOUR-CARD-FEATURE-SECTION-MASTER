# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Frontend Mentor - Four card feature section solution](#frontend-mentor---four-card-feature-section-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
  - [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](/design-samples/desktop-design.png)
![](/design-samples/mobile-design.png)

### Links

- Solution URL: [Solution URL]([https://github.com/savvykhai/FOUR-CARD-FEATURE-SECTION-MASTER.git)
- Live Site URL: [live Site URL](https://four-card-feature-section-master-8m5qw190o-savvykhai.vercel.app)

****## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned
I struggled with figuring out how to make the article with the class .cyan and .orange appear at the center  of the page as a whole, so i sought for help and discoverd i needed to wrap them both around a container so i wraped a section around them this made them appear as a single element on the page therefore making the other element staying by the side. See code below...

```html
        <section class="middle__container">
            <article class="article cyan">
                <h3 class="main__h3">Team Builder</h3>
                <p class="main__p">Scans our talent network to create the optimal team for your project</p>
                <figure class="figure">
                    <img src="images/icon-team-builder.svg" alt="Icon team" width="64" height="64">
                    <figcaption class="offscreen">Icon team</figcaption>
                </figure>
            </article>

            <article class="article orange">
                <h3 class="main__h3">Karma</h3>
                <p class="main__p">Regularly evalutes our talent to ensure quality</p>
                <figure class="figure">
                    <img src="images/icon-karma.svg" alt="Icon karma" width="64" height="64">
                    <figcaption class="offscreen">Icon karma</figcaption>
                </figure>
            </article>
        </section>
```
```css
.middle__container {
    display: grid;
    gap: 1rem;
}
```

I also learnt how to break lines using css. This is done by wraping a span element around the line you want to break, use a unique class name on the span element in case you used it elsewhere then applying css as follows.

```css 
.selector::after {
  content: "\a";
  white-space: pre;
}

### Continued development

I will be focusing on making responsive sites in the future applying flexbox and grid layout. 

## Author

- Frontend Mentor - [@savvykhai](https://www.frontendmentor.io/profile/savvykhai)
- Twitter - [@savvykhai](https://www.twitter.com/savvykhai)
