# Read: 10 - JS Debugging:

- in this chapter we will learn about debugging code and how to find error and fix it .
  we will learn about

# here is what you shouls consider to use when you are facing aproblem or error with your code :

1.  THE CONSOLE & DEV TOOLS
2.  COMMON PROBLEMS
3.  HANDLING ERRORS

![Debugging tools](https://developers.google.com/web/tools/chrome-devtools/javascript/imgs/sources-annotated.png)

![Debugging tools](https://commandlinefanatic.com/art035f002.png)

## errors types in js :

![Debugging tools](https://www.tutsmake.com/wp-content/uploads/2020/05/Types-of-Errors-In-JavaScript.jpeg)

**example**
![Debugging tools](https://scontent.famm3-3.fna.fbcdn.net/v/t1.15752-9/160505418_468691634164769_8417252964819603234_n.jpg?_nc_cat=111&ccb=1-3&_nc_sid=ae9488&_nc_eui2=AeEkNlxarJt2jtEpdqrCKmX00zefNXBq0drTN581cGrR2unXiOy6-5TjeAohyRsy8hPzAZXt-0zOEzZXL3cyPBmr&_nc_ohc=X6Mxjx2CspcAX8Uadzb&_nc_ht=scontent.famm3-3.fna&oh=bda159adabfc2e7a5743de2c235cb71f&oe=6071CEB4)

# HOW TO DEAL WITH ERRORS :

1. DEBUG THE SCRIPT TO FIX ERRORS
   If you come across an error while writing a script
   (or when someone reports a bug), you will need to
   debug the code, track down the source of the error,
   and fix it.
   You will find that the developer tools available in
   every major modern browser will help you with
   this task. In this chapter, you will learn about the
   developer tools in Chrome and Firefox. (The tools in
   Chrome are identical to those in Opera.)
   IE and Safari also have their own tools (but there is
   not space to cover them all).

2. HANDLE ERRORS GRACEFULLY
   You can handle errors gracefully using try, catch,
   throw, and f i na 1 ly statements.
   Sometimes, an error may occur in the script for a
   reason beyond your control. For example, you might
   request data from a third party, and their server
   may not respond. In such cases, it is particularly
   important to write error-handling code.
   In the latter part of the chapter, you will learn how to
   gracefully check whether something will work, and
   offer an alternative option if it fails.

   # when you know the error you will face :

- If you know that you are going to face an error you can handel it using (try, catch, finally statements).

  ![Debugging tools](https://i.ytimg.com/vi/GYWUr7xlK-w/maxresdefault.jpg)

## Summary :

- If you understand execution contexts (which have two
  stages) and stacks, you are more likely to find the error
  in your code.
- Debugging is the process of finding errors. It involves a
  process of deduction.
- The console helps narrow down the area in which the
  error is located, so you can try to find the exact error.
  JavaScript has 7 different types of errors. Each creates
  its own error object, which can tell you its line number and gives a description of the error.
- If you know that you may get an error, you can handle
  it gracefully using the try, catch, finally statements.
  Use them to give your users helpful feedback.
