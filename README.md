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
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](images/solution.png)

### Links

- Solution:([Solution](https://www.frontendmentor.io/solutions/nft-preview-card-challenge-oDNOGcK5nk))
- Live Site:([Live Site](https://devtruce.github.io/nft-preview-card/))

## My process

I had a fun time with this challenge and it was great to help get some real practice while
learning, I enjoyed using flexbox to layout the elements and for the most part I think I did the
challenge relatively well for where I am at in my learning journey. I revisited and reworked
this challenge and I think I did better the second time around for sure, elements are responding
much better and I learned how to correctly get the hover effect!

### What I learned

I learned how to better use html,css & flex box to position elements for a responsive layout, I learned was how to display an altered background/image over an existing one, based on the users actions & I also learned how to correctly use root, html, body & \* selectors. I learned how to
use css to create a nice image overlay! Lastly I learned how valuable this simple debug tool is!
it allowed me to get a better understanding of how my elements are behaving to allow me to better
adjust them.

```css
* {
  border: 2px solid red;
}
```

### Built with

- HTML5
- CSS3
- Flexbox

```html
<div class="nft-image">
  <a
    href="https://www.theverge.com/22310188/nft-explainer-what-is-blockchain-crypto-art-faq"
    target="_blank"
    class="nft-image-hover"
  ></a>
</div>
```

```css
.nft-image {
  width: 100%;
  height: 300px;
  border-radius: 0.75rem;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url(../images/image-equilibrium.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

.nft-image-hover {
  background-color: #00fff48f;
  background-image: url(../images/icon-view.svg);
  background-repeat: no-repeat;
  background-position: center;
  opacity: 0.5;
  border-radius: 10px;
  height: 100%;
  width: 100%;
  cursor: pointer;
  opacity: 0;
  transition: all 250ms ease-in-out;
}

.nft-image-hover:hover {
  opacity: 1;
}
```

### Continued development

I am starting to get better and more confortable with flexbox, units and overall
layout/positioning but this is still my main focus!

### Useful resources

- [CSS Root vs html vs \* vs body](https://blog.timonwa.com/all-vs-root-vs-html-vs-body-selectors) - This helped me better understand how to correctly use root, html, body & \* selectors, this resource also taught me a very simple but helpful trick
  which is to use a simple debug tool.

```css
* {
  border: 2px solid red;
}
```

## Author

- Frontend Mentor - [@DevTruce](https://www.frontendmentor.io/profile/DevTruce)

## Acknowledgments

grace
