# Frontend Mentor - Results summary component solution

This is a solution to the [Results summary component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

<!-- Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge. -->

[Trick](https://www.aleksandrhovhannisyan.com/blog/62-5-percent-font-size-trick/) for never setting pixel font sizes and making them easier to compute in your head:

```css
html {
    font-size: 62.5%;
}

div {
  font-size: 1.8rem; /* This will be 18px */
}
```

Gained a better understanding of css selectors, in particular using [selector lists](https://developer.mozilla.org/en-US/docs/Web/CSS/Selector_list) and the [:is()](https://developer.mozilla.org/en-US/docs/Web/CSS/:is) pseudo-class to create a forgiving selector list.

Clip paths and creation of a circle with a gradient:

```css
.circle-gradient {
    background: #4d21c9;
    background: linear-gradient(to bottom, rgba(77,33,201,1) 0%, rgba(37,33,201,0) 100%);
    clip-path: circle(40%);
    min-width: 24rem;
    min-height: 24rem;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-flow: column;
}
```
```html
<div class="circle-gradient">
  <h1>76</h1>
  <p><strong>of 100</strong></p>
</div>
```

todo: add screenshot

Process-wise, it's helpful to look through all the colors and font sizes in the figma at the start of the project and create the variables. That makes it quicker 

A powerful way to use CSS variables is to create variables based on other variables. This can be useful for keeping track of color schemes and to keep CSS rules modular.  It can help to avoid needing complex / specific css rules and keep things more general. For example, if there are multiple h2, h3, p across the project but each section has a different color scheme, redifining the color scheme in variables for each section might be a good idea instead of adding more css selectors.

todo: add an example of how we're re-defining css variables to style the different parts of the component instead of using complex css rules.

<!-- ```html
<h1>Some HTML code I'm proud of</h1>
``` -->

<!-- ```js
const proudOfThisFunc = () => {
  console.log('🎉')
}
``` -->

<!-- If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more. -->

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
