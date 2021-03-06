Rounded Images
Use the border-radius property to create rounded images:
Example
Rounded Image:
img {
  border-radius: 8px;
}
Try it Yourself »
Example
Circled Image:
img {
 border-radius: 50%;
}
Try it Yourself »
Thumbnail Images
Use the border property to create thumbnail images.
Thumbnail Image:
Example
img {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 5px;
  width: 150px;
}
Try it Yourself »
Thumbnail Image as Link:
Example
img {
 border: 1px solid #ddd;
  border-radius: 4px;
 padding: 5px;
  width: 150px;
}
img:hover {
 box-shadow: 0 0 2px 1px rgba(0, 140, 186, 0.5);
}
Try it Yourself »
ADVERTISEMENT
Responsive Images
Responsive images will automatically adjust to fit the size of the screen.
Resize the browser window to see the effect:
If you want an image to scale down if it has to, but never scale up to be larger than its original size, add the following:
Example
img {
 max-width: 100%;
 height: auto;
}
Try it Yourself »
Tip: Read more about Responsive Web Design in our CSS RWD Tutorial.
Center an Image
To center an image, set left and right margin to auto and make it into a block element:
Example
img {
  display: block;
 margin-left: auto;
 margin-right: auto;
 width: 50%;
}
Try it Yourself »
Polaroid Images / Cards
Cinque Terre
Northern Lights
Example
div.polaroid {
 width: 80%;
  background-color: white;
 box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}
img {width: 100%}
div.container {
 text-align: center;
  padding: 10px 20px;
}
Try it Yourself »
Transparent Image
The opacity property can take a value from 0.0 - 1.0. The lower value, the more transparent:
opacity 0.2
opacity 0.5
opacity 1
(default)
Example
img {
 opacity: 0.5;
}
Try it Yourself »
Image Text
How to position text in an image:
Example
Bottom Left
Top Left
Top Right
Bottom Right
Centered
Try it Yourself:
Top Left » Top Right » Bottom Left » Bottom Right » Centered »
Image Filters
The CSS filter property adds visual effects (like blur and saturation) to an element.
Note: The filter property is not supported in Internet Explorer or Edge 12.
Example
Change the color of all images to black and white (100% gray):
img {
  filter: grayscale(100%);
}
Try it Yourself »
Tip: Go to our CSS filter Reference to learn more about CSS filters.
Image Hover Overlay
Create an overlay effect on hover:
Example
Fade in text:
Hello World
Try it Yourself »
Example
Fade in a box:
John
Try it Yourself »
Example
Slide in (top):
Hello World
Try it Yourself »
Example
Slide in (bottom):
Hello World
Try it Yourself »
Example
Slide in (left):
Hello World
Try it Yourself »
Example
Slide in (right):
Hello World
Try it Yourself »
Flip an Image
Move your mouse over the image:
Example
img:hover {
 transform: scaleX(-1);
}
Try it Yourself »
Responsive Image Gallery
CSS can be used to create image galleries. This example use media queries to re-arrange the images on different screen sizes. Resize the browser window to see the effect:
Add a description of the image here
Add a description of the image here
Add a description of the image here
Add a description of the image here
Example
.responsive {
 padding: 0 6px;
  float: left;
  width: 24.99999%;
}
@media only screen and (max-width: 700px){
  .responsive {
   width: 49.99999%;
    margin: 6px 0;
  }
}
@media only screen and (max-width: 500px){
  .responsive {
    width: 100%;
  }
}
Try it Yourself »
Tip: Read more about Responsive Web Design in our CSS RWD Tutorial.
Image Modal (Advanced)
This is an example to demonstrate how CSS and JavaScript can work together.
First, use CSS to create a modal window (dialog box), and hide it by default.
Then, use a JavaScript to show the modal window and to display the image inside the modal, when a user clicks on the image:
Example
// Get the modal
var modal = document.getElementById('myModal');
// Get the image and insert it inside the modal - use its "alt" text as a caption
var img = document.getElementById('myImg');
var modalImg = document.getElementById("img01");
var captionText = document.getElementById("caption");
img.onclick = function(){
 modal.style.display = "block";
  modalImg.src = this.src;
  captionText.innerHTML = this.alt;
}
// Get the <span> element that closes the modal
var span = document.getElementsByClassName("close")[0];
// When the user clicks on <span> (x), close the modal
span.onclick = function() {
 modal.style.display = "none";
}c