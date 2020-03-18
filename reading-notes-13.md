# Reading Notes 12      

[Reading-01](reading-notes.md)  

**Local Storage**  
- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.  

-  Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).  
- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.  

**HTML Storage**  
- what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.  
- This data is never transmitted to the remote web server.  

**USING HTML5 STORAGE**  

- HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string.  
- If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.
    - interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};  
- Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets.  


**TRACKING CHANGES**  
- If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.  
