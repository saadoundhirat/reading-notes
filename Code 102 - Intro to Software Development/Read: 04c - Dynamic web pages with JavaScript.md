
# **what i have learned:**
* JavaScript is the world's most popular programming language.
* JavaScript is the programming language of the Web.
* JavaScript is easy to learn.
* This help you understand the basics of this programing language

 # **Why Study JavaScript?**
JavaScript is one of the 3 languages all web developers must learn:
1. HTML to define the content of web pages
2. CSS to specify the layout of web pages 
3. JavaScript to program the behavior of web pages

 # How to connect your JavaScript file with html page :

 *Using the script tag to include an external JavaScript file
To include an external JavaScript file, we can use the script tag with the attribute src. You've already used the src attribute when using images. The value for the src attribute should be the path to your JavaScript file.
  <em><script type="text/javascript" src="path-to-javascript-file.js"></script></em>
   This script tag should be included between the <head> tags in your HTML document.

# **JavaScript Files** 
 * JavaScript files are not HTML files or CSS files.
 * Always end with the js extension
 * Only include JavaScript
 * It's customary to put all JavaScript files in a folder called js on websites, like so: 

# **JavaScript Data Types:**
* In programming, data types is an important concept.
* To be able to operate on variables, it is important to know something about the type.

* **data types:**
* String:	represents sequence of characters e.g. "hello"
* Number:represents numeric values e.g. 100
* Boolean:represents boolean value either false or true
* Undefined:represents undefined value
* Null:represents null i.e. no value at all

# **LINKING TO A JAVASCRIPT FILE FROM AN HTML PAGE:*
 1. Create a folder to put the example in called cOl, then start up your favorite code editor, and enter the text to the right. 
     A JavaScript file is just a text file (like HTML and CSS files are) but it has a . j s file extension, so save this file with
      the name add-content .js 

 2. Get the CSS and images for this example from the website that accompanies the book:
        <em>www.javascriptbook. com</em>
    To keep the files organized, in the same way that CSS files often live in a folder called styles or css, your JavaScript files can live in a folder called
    scripts,javascript,orjs.
    In this case, save your file in a folder called js.

 3. In your code editor, enter the HTML shown on the left. Save this file with the name add-content.html
     The HTML script element is used to load the JavaScript file into the page. It has an attribute called src, whose value is the
     path to the script you created.
   This tells the browser to find and load the script file (just like the src attribute on an img tag). 

 4. Open the HTML file in your browser. You should see that the JavaScript has added a greeting (in this case, Good Afternoon!) to    the page. (These greetings are coming from the JavaScript file;
   they are not in the HTML file.)   

 5.  Once you have tried the example in your browser, view the source code for the page.
    (This option is usually under the View, Tools or Develop menu of
    the browser.)  

 6. The source of the web page does not actually show the new element that has been added
     into the page; it just shows the link to the JavaScript file. 

 7. Finally, try opening the HTML file, removing the src attribute from the opening
    script tag, and adding the new code shown on the left between the opening scripttag and the closing scripttag.
    The s re attribute is no longer needed because the
    JavaScript is in the HTML page.       
     

![js](https://blog.codeanalogies.com/wp-content/uploads/h5p/content/2/images/imageAfter-5aefc26211941.png)