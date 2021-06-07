# Passing Functions as Props 

### What does .map() return?
 * answer: its return an array that has the same number of elements that the original array have.
### If I want to loop through an array and display each value in JSX, how do I do that in React?
 * answer: same as in js where we define an variable thats has the returns values then we use it inside the render => return function to render each element in the array but we write the javascript code inside {} in JSX.
### Each list item needs a unique ?
 * answer:__key passed as props and we mostlly use index of the item or an Id if we have one inside the object__.
### What is the purpose of a key?
  * answer: to make each object that we make from the component unique.
 ___
 ## Spread Operator (…) in JavaScript:
 * Spread Operator The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
 ![Click Here](https://miro.medium.com/max/3208/1*ck6Fs5k54T8Yv09D2dS0jA.png)


### What is the spread operator?
 * Spread Operator The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.
### List 4 things that the spread operator can do. 
     * answer:
     1-adding items to arrays
     2-combining arrays
     3-combining objects
     4-spreading an array out into a function’s arguments
     5-passing arrays by value 
### Give an example of using the spread operator to combine two arrays.
  * answer: 
### Give an example of using the spread operator to add a new item to an array.
  * answer: `

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

`
### Give an example of using the spread operator to combine two objects into one.
  * answer: ` const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }
`
 ___

 ### resources:
recource      | links
------------- | -------------
Spread Operator    | [Link](https://www.google.com/url?sa=i&url=https%3A%2F%2Fjavascript.plainenglish.io%2F8-ways-to-use-spread-operator-in-javascript-b66fcf016efe&psig=AOvVaw3EiC8eCn6m3WxU9m6a6mk2&ust=1623189818704000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCIDfwrfDhvECFQAAAAAdAAAAABAD)
React State Vs Props | [Link]() |