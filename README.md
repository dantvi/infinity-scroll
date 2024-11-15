# Infinite Scroll

This project is an infinite scroll image gallery built as part of the course "JavaScript Web Projects: 20 Projects to Build Your Portfolio" by Zero To Mastery. It uses the Unsplash API to fetch and display random images, loading more images automatically as the user scrolls.

## Table of contents

- [Infinite Scroll](#infinite-scroll)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Useful resources](#useful-resources)
  - [Author](#author)
  - [Acknowledgments](#acknowledgments)

## Overview

This project allows users to:
- View a continuous feed of random images from Unsplash.
- Load new images automatically as they scroll down the page.
- Click on images to view them on Unsplash in a new tab.

### Screenshot

![](./screenshot.png)

### Links

- Live Site URL: [DT Code](https://infinity-scroll.dtcode.se/)

## My process

### Built with

- HTML5 for structure
- CSS3 for styling, including responsive design with media queries
- JavaScript (ES6+) for functionality
- Fetch API to retrieve images from the Unsplash API
- Unsplash API for image sourcing

### What I learned

In this project, I learned how to implement infinite scrolling with the Unsplash API. I improved my understanding of asynchronous JavaScript by handling API requests with async/await and adding event listeners for scroll events to dynamically load more content as the user scrolls.

Example code for loading images from the Unsplash API:

```js
async function getPhotos() {
    try {
        const response = await fetch(apiUrl);
        photosArray = await response.json();
        displayPhotos();
    } catch (error) {
        console.log(error);
    }
}
```

### Useful resources

- [Unsplash API Documentation](https://unsplash.com/documentation) - This was essential for understanding how to work with the API and set up the image requests.
- [JavaScript Fetch API Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) - A helpful guide to understand how to retrieve data asynchronously.

## Author

- GitHub - [@dantvi](https://github.com/dantvi)
- LinkedIn - [@danieltving](https://www.linkedin.com/in/danieltving/)

## Acknowledgments

Special thanks to Zero To Mastery for providing the project structure and guidance throughout the course.
