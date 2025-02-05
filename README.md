# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [The challenge](#the-challenge)
- [Screenshots](#screenshots)
  - [1. Desktop version](#1-desktop-version)
  - [2. Mobile version](#2-mobile-version)
- [PageSpeed Insights results](#pagespeed-insights-results)
- [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Tested with](#tested-with)
  - [What I learned](#what-i-learned)
- [Acknowledgement](#acknowledgement)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshots

##### 1. Desktop version

Default state
![Social links profile - default](./assets/screenshots/desktop/Social-links-profile-default.png)

Hover state
![Social links profile - hover](./assets/screenshots/desktop/Social-links-profile-hover.png)

##### 2. Mobile version

Default state
![Social links profile - default](./assets/screenshots/mobile/Social-links-profile-default.jpg)

Active state
![Social links profile - active](./assets/screenshots/mobile/Social-links-profile-active.jpg)

### PageSpeed Insights results

[Mobile version](https://pagespeed.web.dev/analysis/https-rupali317-github-io-social-links-profile-main/ca6guo7umb?form_factor=mobile)

[Desktop version](https://pagespeed.web.dev/analysis/https-rupali317-github-io-social-links-profile-main/ca6guo7umb?form_factor=desktop)

### Links

- Solution URL: [Social links profile Github solution](https://github.com/rupali317/social-links-profile-main)
- Live Site URL: [Social links profile live URL](https://rupali317.github.io/social-links-profile-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- [Github Pages](https://pages.github.com/) - Allows to host static websites directly from a GitHub repository.

### Tested with

- Browsers used for testing: Google Chrome, Firefox, Safari, Brave, Microsoft Edge.
- Devices:
  - (Real) MacBook Pro (14-inch), Samsung Galaxy A33 5G, Samsung Galaxy S20+, iPad Air (13-inch), MacBook Pro (13-inch).
  - (Virtual) The mobile and tablet devices mentioned under Chrome's dev console.
- Screen reader: MacOS VoiceOver.

### What I learned

- Understood the concepts/importance related to `noreferrer` and `noopener`. Opening a link as a target blank forms a connection between child tab (new tab) and parent tab (old tab) where the new tab has access to the information from the old tab. Without the `noopener` the new tab can redirect the old tab to a malicious site by modifying `window.opener.location`, which will target the old tab. Without the `noreferrer`, the new tab has access to the old tab's URL and can have access to sensitive information. However some browsers may have these protections in-built without requiring us to explicitly state the values.

```html
<a
  href="https://github.com/"
  aria-label="Visit Jessica's GitHub"
  target="_blank"
  rel="noopener noreferrer"
  >GitHub</a
>
```

- There is a subtle difference between `width: inherit` and `width: 100%`. If the parent does not have an explicitly defined width, width: 100% will still fill the available space, while width: inherit will be more dependent on the parent's explicit width, otherwise the container with `width: inherit` will be auto if the parent's width is not stated.

## Acknowledgement

- In all my projects, I always refer to CSS reset to provide a clean/consistent slate for the CSS stylings across all the browsers. [Joshua's CSS reset](https://www.joshwcomeau.com/css/custom-css-reset/), [Andy Bell's CSS reset](https://piccalil.li/blog/a-more-modern-css-reset/)
- I express my gratitude towards my mentor - Deborah for the insightful code review session and for suggesting improvements.

## Author

- Linkedin profile - [Rupali Roy Choudhury](https://www.linkedin.com/in/rupali-rc/)
- Frontend Mentor - [@rupali317](https://www.frontendmentor.io/profile/rupali317)
