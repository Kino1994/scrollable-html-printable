# Make Scrollable HTML Printable as PDF with all text

To make scrollable HTML (even with nested scroll areas) printable as a PDF, execute the following code in your web browser's console.

There is no need to manually expand any scrollable areas beforehand, as the code will handle this automatically.

```
// Select all div elements on the page
var divs = document.querySelectorAll('div');

// Iterate over each div and modify its style
divs.forEach(function(div) {
    div.style.overflow = 'visible';  // Ensure all content is displayed without scroll
    div.style.height = 'auto';       // Set the div height to automatically fit the content
    div.style.maxHeight = 'none';    // Remove any maximum height restrictions
});
```
