# Reading Notes 12      

[Reading-01](reading-notes.md)  

_**Chart.js docs**_  

_Creating a Chart Example Code_  

- https://www.chartjs.org/docs/latest/  

-  `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.  

-  As a consequence of the way fallback is provided, unlike the `<img>` element, the `<canvas>` element requires the closing tag (`</canvas>`). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.  

- The script includes a function called draw`()`, which is executed once the page finishes loading; this is done by listening for the load event on the document. This function, or one like it, could also be called using window.setTimeout`()`, window.setInterval`()`, or any other event handler, as long as the page has been loaded first.  

- Unlike SVG, `<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths.  

- In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

- __globalAlpha = transparencyValue__  
Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.  

- The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors.  

- Because the strokeStyle and fillStyle properties accept CSS rgba color values, we can use the following notation to assign a transparent color to them.

- The canvas rendering context provides two methods to render text:

    - fillText(text, x, y [, maxWidth])  
    Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.  
    strokeText(text, x, y [, maxWidth])  
    Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.  

