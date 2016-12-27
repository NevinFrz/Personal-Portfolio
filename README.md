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

### PageSpeed Insights Score
* Mobile - 93/100
* Desktop - 94/100
