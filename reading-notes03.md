# Reading Notes 03

_Types of Lists in HTML / CSS_
- **Ordered lists** : are lists where each item in the list is.
numbered. This would be used when you need to list things out in a numbered order. May be for baking or like instructions to build something. 
- **Unordered lists** : are lists that begin with a bullet point.
You would use this for just laying out ideas and making bullet points.  

- **Definition lists** : are made up of a set of terms along with the definitions for each of those terms.  

**_Ordered list_** is created with the `<ol>` element then will have the `<li>` inside of the `<ol>` tag.  
**_Unordered list_**  is created with the `<ul>` element. Then would follow with the `<li>` element.  
`<dl>` consists of a series of terms and
their definitions.  
`<dt>` This is used to contain the term
being defined (the definition
term).  
`<dd>` This is used to contain the
definition.   
**Nesting** : Nesting is important because it helps reading the code that is written. It also shows proper etiquette.  

**Boxes** : In CSS you can create and control boxes. To
set your own dimensions for a box you can use the height and
width properties. The most popular ways to specify the size of a box are to use pixels or percentages.  All you need to do is to call out the tag in CSS and then use height: 123px; same for width. You can also do cool stuff with these boxes by setting min-height and min-width. It gets pretty crazy to the point of where you can control weather the box expands or contrasts when the user enlarges or shrinks the window.   

**hidden** and **scroll** are both self explanatory I feel. Here is an example: overflow: hidden; and the same for scroll overflow: scroll; .  

**borders, margin and padding** now this is something that I struggle with. This is something that allows you to control and set the properties of each of these. Just thing how a picture sits inside a frame and then adds another frame around it. One would represent a border. The next frame would be the margin and the inside from the frame to the picture is the padding. You can set the amount of buffering between the both of them. Yes, you can add even more style to all of these like lined , dotted, colored and so on so forth. It can get creative very quickly.  

**Centering Content**  That's right you guessed it! You can also set the position of your content. Pretty straight forward but like anything else, you may be faced with challenges.  

**JS Loops** : Operators and Loops Comparisons
There are different way to make a comparison in a loop Here are a few examples:

== is equal to  
!= is not equal to  
=== strict equal to  
!== strict not equal to  
. > greater than  
ignore period above before the greater than

< less than  
. >= greater than or equal to  
<= less than or equal to  
&& logical and  
|| logical or  
! logical not  
Some examples of logical and / or const a = 3; const b = -2;

console.log(a > 0 && b > 0); // expected output: false

console.log(a > 0 || b > 0); // expected output: true

console.log(!(a > 0 || b > 0));

Loops

**_for loop_**
for (let step = 0; step < 5; step++) { // Runs 5 times, with values of step 0 through 4. console.log('Walking east one step'); }  


while
let n = 0; let x = 0; while (n < 3) { n++; x += n; }


