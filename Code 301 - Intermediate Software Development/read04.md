# Readings: React and Forms

- **What is a ‘Controlled Component’?**
 * **Answer:** 
 A Controlled Component: is one that takes its current value through props and notifies changes through callbacks like onChange. A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component. You could also call this a "dumb component".
 </br>
 A Uncontrolled Component is one that stores its own state internally, and you query the DOM using a ref to find its current value when you need it. This is a bit more like traditional HTML.

 ```
// Controlled:
<input type="text" value={value} onChange={handleChange} />

// Uncontrolled:
<input type="text" defaultValue="foo" ref={inputRef} />
// Use `inputRef.current.value` to read the current value of <input>
```



- **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**
**Answer:** depends of the case that we use the state value, in most cases we should update the state as soon as they enter the value using callback function since we are using (controlled component).



- **How do we target what the user is entering if we have an event handler on an input field?**
**Answer:** 
using event target method to target the name of the form field and get the data from state.
___


- **Why would we use a ternary operator?**
    **Answer:** its make the code easier to understand with less lines of code, in most cases we only use (if and else only) because its hard to understand elseif with this way.
- **Rewrite the following statement using a ternary statement:**
    **Answer:** 


    ```
      if(x===y){
        console.log(true);
        } else {
        console.log(false);
        }

    ```    

    ```
      (x===y) ? console.log(true) : console.log(false);

    ```
___
### resources:
recource      | links
------------- | -------------
Controlled Component    | [Link](https://stackoverflow.com/questions/42522515/what-are-react-controlled-components-and-uncontrolled-components)
React Forms | [Link](https://reactjs.org/docs/forms.html) |
The Conditional (Ternary) Operator Explained | [Link](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff) |