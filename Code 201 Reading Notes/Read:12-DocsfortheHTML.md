# Read: 12 - Docs for the HTML <canvas> Element & Chart.

# Charts :

- charts used to display data visually some pepole prefer them but i dont really but for some people they are easier to look at but its hard to make them for sure.

> **Chart javascript**: they are pluged in with java and they use html5 canvas to draw the graph onyo the page.

- then we plug in charts js to our files the use the script to add that file to our html files.

* to draw line we need to use canvas:
 `<canvas id="buyers" width="600" height="400"></canvas>`
* next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:
`<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>`
 * then : 
 `var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}`


# types of charts we can draw :
 1. Drawing a line chart
 2. Drawing a pie chart
 3. Drawing a bar chart

 this link will to see the types:
 [](https://www.webdesignerdepot.com/cdn-origin/uploads7/easily-create-stunning-animated-charts-with-chart-js/chartjs-demo.html)

 > The great things about Chart.js are that it’s simple to use and really very flexible. Plus, once you’ve mastered the basics here, you’ll discover that there are tons of options 


 # canvas API:
  * WE CAN USE THEM FOR
  1. DRAWING SHAPES 
  2. APPLAYING STYLES AND COLORS 
  3. DRAWING TEXT 

  Applying styles and colors
If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

fillStyle = color Sets the style used when filling shapes.
strokeStyle = color Sets the style for shapes’ outlines. color is a string representing a CSS //color>, a gradient object, or a pattern object. We’ll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).
Drawing text
The canvas rendering context provides two methods to render text:

*fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

strokeText(text, x, y [, maxWidth]) Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
A fillText example The text is filled using the current fillStyle.
