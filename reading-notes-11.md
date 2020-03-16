# Reading Notes 11     

[Reading-01](reading-notes.md)  

**Controlling sizes of images in CSS**  

- Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download.   

- Whenever you use consistently sized images across a site, you can use CSS to control the dimensions of the images, instead of putting the dimensions in the HTML.  

**Aligning Images Using CSS**  

- Rather than using the `<img>` element's align attribute, web page authors are increasingly using the float property to align images.  

- The float property is added to the class that was created to represent the size of the image.  

- You can center images by using CSS along with manipulating the borders, margins and padding.  

- You can specify class names that allow any element to be centered, in the same way that you can for the dimensions or alignment of images.

**Background Img**  

- The background-image property allows you to place an image behind any HTML element.  

- The path to the image follows the letters url, and it is put inside parentheses and quotes.  

- You can use other tags to do different effects such as.  
    - repeat  
    - repeat-x  
    - repeat-y  
    - no repeat  
    - fixed  
    - scroll  
**Background Position**  

- When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed.  

    - left top  
    - left center  
    - left bottom  
    - center top  
    - center center  
    - center bottom  
    - right top  
    - right center  
    - right bottom  
- If you only specify one value, the second value will default to center.   