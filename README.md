# Website Performance Optimization project

### The improvements I made in this page are as follows
1. All the files where minified (HTML, CSS, JavaScrpit).
2. All the images where optimized.
3. Async attribute was used in Google Analytics script tags to avoid CRP in `index.html`.
4. The print.css was called with print media query to avoid CRP in `index.html`.
5. External CSS was inlined to avoid CRP in `index.html`.
6. Removed GoogleFonts API to avoid CRP in `index.html`.
7. Eliminated two instances of Forced Synchronous Layouts in `views/js/main.js` that occured while scrolling and changing the size of pizza.
8. Added `will-change: transform;` and `transform: translateZ(0);` under mover class in `views/css/style.css` to create a new layer.
9. Added requestAnimationFrame in `views/js/main.js`.
10. Reduced the number of pizza in the page dynamically with respect the size of screen.

### Instructions on how to perform analysis on the webpage
#### How to check score on PageSpeed Insights
* Open a browser tab or window.
* Go to [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/).
* Paste in the URL of index.html.
* Click on ANALYZE.

#### How To check the frame rate and resize time of the optimized version
* Open up Google Chrome browser.
* Open pizza.html on your browser.
* To open the DevTools
  - Select the Chrome menu at the top-right of your browser window, then select Tools > Developer Tools.
  - Right-click on any page element and select Inspect Element
  - Use CTRL + SHIFT + I or F12 (or CMD + OPT + I on Mac).
* To check the resize time
  - If the console drawer is not visible, click on **>_** at the top-right of the DevTools window.
  - Click the left or size side of the slider.
  - The message `Time to resize pizzas:` followed by the time in milliseconds will display on the console.

* To check the frame rate
  - Click on Timeline in the DevTools menu.
  - To start recording a new timeline, click the record toolbar button at the top-left (below the search button) of the DevTools window, or press CTRL + E.
  - While recording, scroll the Cam's Pizzeria page up and down a few times.
  - Click the record toolbar button or press CTRL + E to stop recording.
  - Select an area of interest in the overview by dragging.  Zoom and pan the timeline with the mousewheel or WASD keys.

### PageSpeed Insights Score
* Mobile - 93/100
* Desktop - 94/100
