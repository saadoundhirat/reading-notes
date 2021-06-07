# more about css layout :

# layout:

- as we know CSS treats each HTML element as if it is in its
  own box. This box will either be a block-level
  box or an inline box

* so there is two type of elements layout :

1. block-level-box :
   Block-level boxes start on a new line and act as the main building blocks of any layout. such as p,h,ul,li
2. inline-box:
   while inline boxes flow between surrounding text. such as img,i,em.

- z-index : allow us to controll which box go on the top.

- Relative positioning moves an element in relation to where it
  would have been in normal flow.

- position:absolute : When the position property is given a value of absolute,the box is taken out of normal
  flow and no longer affects the position of other elements on the page. (They act like it is not there.).

-position:fixed: it positions the element in relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exact same place. It is a good idea to try this example in your browser to see the effect.

float: The float property allows youto take an element in normal flow and place it as far to the
left or right of the containing element as possible.

screen sizes :
page size: Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

Fixed Width Layouts : the screen contant size will not change if end user changed there browser screen size.

![Fixed Width](https://scontent.famm3-3.fna.fbcdn.net/v/t1.15752-9/159980231_241067401052928_4322013055323647218_n.png?_nc_cat=108&ccb=1-3&_nc_sid=ae9488&_nc_eui2=AeF__AYgNjf2BWYoBxtbLpVdQEqruNnVQkVASqu42dVCRcwGctk8exo2oy-KH7dsTCvemRt_YrU6DKHSUO692tEl&_nc_ohc=UrhVWu6XfHwAX8H5cYS&_nc_ht=scontent.famm3-3.fna&oh=d7265bd48a2aad67a6b8fc28c537723b&oe=6073F267)

![Fixed Width](https://www.templatemonster.com/blog/wp-content/uploads/2017/05/fixed-width1.png)

- Liquid Layouts: the contant sizw will change if the user changed his browser size they tend to
  use percentages.

![Fixed Width](https://scontent.famm3-2.fna.fbcdn.net/v/t1.15752-9/159980219_441937173813437_2346756627501683324_n.jpg?_nc_cat=103&ccb=1-3&_nc_sid=ae9488&_nc_eui2=AeGSaJcwDMCgzfXKEEhJ1O94bkPNEgCPa-BuQ80SAI9r4HsuOEnOfJuO5AsHL-q9KTmIJZiJuvVXsTruPtB-7wsQ&_nc_ohc=lttxhdzrL1kAX8c6COQ&_nc_ht=scontent.famm3-2.fna&oh=ca52347e8d5628683c883950061a609a&oe=60734377)

![Fixed Width](https://uploads.sitepoint.com/wp-content/uploads/2011/09/layout-fluid.png)

## CSS Frameworks :

- CSS frameworks aim to make your life easier by providing the code for
  common tasks, such as creating layout grids, styling forms, creating
  printer-friendly versions of pages and so on. You can include the CSS
  framework code in your projects rather than writing the CSS from scratch.

### advantages :

- They save you from
  repeatedly writing code for
  the same tasks.
- They will have been tested
  across different browser
  versions (which helps avoid
  browser bugs).

### disadvantages :

- They often require that you
  use class names in your
  HTML code that only control
  the presentation of the page
  (rather than describe its
  content).
- They often require that you
  use class names in your
  HTML code that only control
  the presentation of the page
  (rather than describe its
  content).

# summary:

- div elements are often used as containing elements
  to group together sections of a page.
- Browsers display pages in normal flow unless you
  specify relative, absolute, or fixed positioning.
- The float property moves content to the left or right
  of the page and can be used to create multi-column
  layouts. (Floated items require a defined width.)
- Pages can be fixed width or liquid (stretchy) layouts.
- Designers keep pages within 960-1000 pixels wide,
  and indicate what the site is about within the top 600
  pixels (to demonstrate its relevance without scrolling).
- Grids help create professional and flexible designs.
- CSS Frameworks provide rules for common tasks.
- You can include multiple CSS files in one page

> quoted from html&css book by Jon Ducket
