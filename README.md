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

![](src/images/solution.png)

### Links

- Solution:([Solution](https://www.frontendmentor.io/solutions/nft-preview-card-challenge-oDNOGcK5nk))
- Live Site:([Live Site](https://devtruce.github.io/nft-preview-card/))

## My process

I had a fun time with this challenge and it was great to help get some real practice while
learning, I enjoyed using flexbox to layout the elements and for the most part I think I did the
challenge relatively well for where I am at in my learning journey. I revisited and reworked
this challenge and I think I did better the second time around for sure, elements are responding
much better and I learned how to correctly get the hover effect!. I revisited the challenge again
to redo the image hover effect with better html, this time around I included an img tag for the
img in the card. I still will like to revist the challenge again once more in the future and
complete the hover effect using the ::before & ::after pseudo selectors but for now this is how
I wanted to go about completing the effect.

### What I learned

I learned how to better use html,css & flex box to position elements for a responsive layout, I learned was how to display an altered background/image over an existing one, based on the users actions & I also learned how to correctly use root, html, body & \* selectors. I learned how to
use css to create a nice image overlay! Lastly I learned how valuable this simple debug tool is!
it allowed me to get a better understanding of how my elements are behaving to allow me to better
adjust them. I also learned that I can set the parent position to relative and the child element
to absolute if I would like to restrict the child size to stay within the parent.

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
<div class="img-container">
  <img
    class="nft-image"
    src="src/images/image-equilibrium.jpg"
    alt="equilibrium"
  />
  <a
    href="https://www.merriam-webster.com/dictionary/equilibrium"
    class="nft-image-hover"
  ></a>
</div>
```

```css
* {
  margin: 0;
  padding: 0;
  text-decoration: none;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  font-size: 1.125rem;
  font-family: "Outfit";
  font-weight: 300;
  color: var(--soft-blue);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: var(--main-bg);
}

.container {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 22rem;
  background-color: var(--card-bg);
  border-radius: 0.75rem;
  overflow: hidden;
  padding: 1.5rem;
  margin: 1rem;
}

.img-container {
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  width: 100%;
  border-radius: 0.75rem;
  position: relative;
}

.nft-image {
  width: 100%;
  display: block;
}

.nft-image-hover {
  position: absolute;
  background-color: #00fff48f;
  background-image: url(../images/icon-view.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 5rem;
  opacity: 0.5;
  border-radius: 10px;
  width: 100%;
  height: 100%;
  cursor: pointer;
  opacity: 0;
  transition: all 350ms ease-in-out;
}

.nft-image-hover:hover,
.nft-image-hover:focus {
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

[Grace Snow](https://github.com/grace-snow)

Massive thank you to Grace for all of the feedback she has provided! I cannot thank her enough!
she has been a great help! Her advice is plentiful and I have learned so much from her already
in the short period of time I have known her.
