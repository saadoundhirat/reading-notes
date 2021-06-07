# what is css : 
* css stands for **cascading style sheet** 
* CSS allows you to create rules that specify how the content of
  an element should appear. For example, you can specify that
  the background of the page is cream, all paragraphs should
  appear in gray using the Arial typeface, or that all level one
  headings should be in a blue, italic, Times typeface.

  ### how css works  :
 **CSS Associates Style rules with HTML elements**
   * CSS works by associating rules with HTML elements. These rules govern
     how the content of specified elements should be displayed. A CSS rule
     contains two parts: a selector and a declaration.
* **Selectors** indicate which
element the rule applies to.
The same rule can apply to
more than one element if you
separate the element names
with commas.

* **Declarations** indicate how
the elements referred to in
the selector should be styled.
Declarations are split into two
parts (a property and a value),
and are separated by a colon.

* **Properties** indicate the aspects
of the element you want to
change. For example, color, font,
width, height and border.

* **Values** specify the settings
you want to use for the chosen
properties. For example, if you
want to specify a color property
then the value is the color you
want the text in these elements
to be.

![html page WireFrames ](https://puzzleweb.ru/en/images/css/1_1.png)

# **Why use External Style Sheets?**
* When building a website there are several advantages to placing your
  CSS rules in a separate style sheet.
* All of your web pages can share
the same style sheet. This is
achieved by using the <link>
element on each HTML page of
your site to link to the same CSS
document. This means that the
same code does not need to be
repeated in every page (which
results in less code and smaller
HTML pages). 

* Therefore, once the user has
downloaded the CSS stylesheet,
the rest of the site will load
faster. If you want to make a
change to how your site appears,
you only need to edit the one
CSS file and all of your pages
will be updated. For example,
you can change the style of
every h1 element by altering
the one CSS style sheet, rather
than changing the CSS rules on
every page. The HTML code
will be easier to read and edit
because it does not have lots of
CSS rules in the same document.
It is generally considered good
practice to have the content of
the site separated from the rules
that determine how it appears.

# **css colors**
## Hexadecimal Colors
* A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the    components of the color. All values must be between 00 and FF.
* p1 {background-color: #ff0000;}   /* red */
* p2 {background-color: #00ff00;}   /* green */
* p3 {background-color: #0000ff;}   /* blue */

* Colors in CSS can be specified by the following methods:
1. Hexadecimal colors
2. Hexadecimal colors with transparency
3. RGB colors
4. RGBA colors
5. HSL colors
6. HSLA colors
7. Predefined/Cross-browser color names
8. With the currentcolor keyword
 ### this image will show you how to color using hexa and decimal :
![color using hexa and decimal](https://cdn.educba.com/academy/wp-content/uploads/2020/03/CSS-Color-Codes.jpg)

# **Summary**

* **CSS treats each HTML element as if it appears inside
its own box and uses rules to indicate how that
element should look.**

* **Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
X Different types of selectors allow you to target your
rules at different elements.**

* **Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.**

* **CSS rules usually appear in a separate document,
although they may appear within an HTML page.**