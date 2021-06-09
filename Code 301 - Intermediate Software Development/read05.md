 # Readings: React and Forms

## **How would you break a mock into a component heirarchy?**
 * **Answer:** we divide the component hierarchy to make each component do only on thing (single responsibility principle) then we write it usign function or objects, but If it ends up growing, it should be decomposed into smaller subcomponents.
## **What is the single responsibility principle and how does it apply to components?**
* **Answer:** make each component do only on thing (single responsibility principle) then we write it usign function or objects, but If it ends up growing, it should be decomposed into smaller subcomponents.
## **What does it mean to build a ‘static’ version of your application?**
* **Answer:** to build all the components hierarchy without any interactivity with other component only use props (no state used)
## **Once you have a static application, what do you need to add?**
* **Answer:**To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props.
## **What are the three questions you can ask to determine if something is state?**
* **Answer:**
1Is it passed in from a parent via props? If so, it probably isn’t state.
2Does it remain unchanged over time? If so, it probably isn’t state.
3Can you compute it based on any other state or props in your component? If so, it isn’t state.
## **How can you identify where state needs to live?**
* **Answer:**
1. Identify every component that renders something based on that s. Find a common owner component (a single component above all the components that need the stahe hierar. Either the common owner or another component higher up in the hierarchy should own the state.
4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

![Thinking in React](https://miro.medium.com/max/1705/1*Dee4cg5Hzg7JME1A9tjZJQ.png)
___
### resources:
recource      | links
------------- | -------------
Thinking in React   | [Link](https://reactjs.org/docs/thinking-in-react.html)
React tree | [Link](https://reactjs.org/docs/forms.html) |
The Conditional (Ternary) Operator Explained | [Link](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2F%40nimelrian%2Fthinking-in-react-a-paradox-statement-33c19e2eb9e2&psig=AOvVaw3EjXC2O_pMM6YFR6u6aPf3&ust=1623363712606000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCMiCyaHLi_ECFQAAAAAdAAAAABAD) |