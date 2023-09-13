# Dynamic Photo Loader

This project fetches random photos from the Unsplash API and dynamically displays them as the user scrolls down the page.

## Features

- Fetches random photos from the Unsplash API.
- Dynamically displays photos as the user scrolls down the page.

## API Documentation
This project uses the Unsplash API to fetch random photos. For more information on the API, refer to the Unsplash API Documentation.

## Hosted Link
  https://ameya-shinde.github.io/Infinite-Pictures-Scroll/

## JS Functionality
* `async function getPhotos() { ... }`: This is an asynchronous function for fetching and displaying photos.
* `try-catch`: This block handles any errors that may occur during the execution of the code inside the try block.
* `await fetch(apiUrl)`: It makes an asynchronous request to the apiUrl using the fetch API.
* `document.getElementById('loader').style.display = 'none';`: This line hides the loader element once the photos are loaded.
* `const item = document.createElement("div");`: Creates a div element to hold the image.
* `img.setAttribute("src", photo.urls.small);`: Sets the src attribute of the image element to the URL of the photo.
* `item.appendChild(img);`: Appends the image element to the item div.
* `window.addEventListener("scroll", () => { ... });`: Adds an event listener for the "scroll" event on the window.
* `window.scrollY + window.innerHeight`: The current vertical position of the scroll plus the height of the viewport.
* `document.documentElement.scrollHeight` : The total height of the document.
* `if (window.scrollY + window.innerHeight >= document.documentElement.scrollHeight) { ... }`: Checks if the user has scrolled to the bottom of the page. If true, it calls getPhotos() to load more photos.

This code combines the use of asynchronous JavaScript, event handling, DOM manipulation, and API fetching to dynamically load and display photos from the Unsplash API as the user scrolls down the page.
