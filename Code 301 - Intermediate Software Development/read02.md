# State and Props :


## React life cycle events : 

1- mounting: this is when react component added to the Dom t occurs during the mounting phase.
2- Updating (set.State) : here where the componet value is changed from user interaction in the UI (Here it will re-render the component).
3- unmounting : when a component is being removed from the DOM.

## constructor in react component :

 ** in react costructor is being or initialize before the render methode so thats means it will be called before the mounting where the component will be add to the DOM.
 ** we dont call the set.State method inside the render functions it called inside the component class.
 ** `class FishTableRow extends React.Component {
        constructor() {
        super(props); //gives us access to props
        //Don’t call this.setState() here
        this.state = { //intitialize local state
        showDescription: false
        }; }`

 ** NOTE: dont use set.State inside the constructor because it will lead to problems and cuz an issues so, Doing this will ignore all updates to props, so it shouldn’t be done unless it is intentional. 

 ## React lifecycle qustions : 
  1- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
      
      ** answer: ‘render’ because it we be added to the dom (mounting) after it render what its inside it (JSX) JSX stands for JavaScript XML (eXtensible Markup Language).

  2- What is the very first thing to happen in the lifecycle of React?

      ** answer:  static getDerivedStateFromProps() The static getDerivedStateFromProps is the first React lifecycle method to be invoked during the updating phase.

  3-  put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

        ** answer: 
        1- constructor
        3- render
        2- React Updates
        4- componentDidMount
        5- componentWillUnmount

  4- What does componentDidMount do?
       
       ** answer: This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().
       ** note: set.state can be called here but make sure about the performance because it can take to mush time since this will lead to re-rendering the component.

  ## React State Vs Props:
  1-What types of things can you pass in the props?
    ** answer: Functions parameters arguments

  2-What is the big difference between props and state?
    ** answer: 
    - props: is been passed to the component thats means its been handels outside the component.
    - state: is been declaerd and handeled inside the component it self.

  3-When do we re-render our application?
    ** answer: when the state of the component is changed.

  4-What are some examples of things that we could store in state?
    ** answer: - Forms & Counters or anythig will be handeld inside the component.


# resources:
recource      | links
------------- | -------------
React lifecycle      | [Link](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
React State Vs Props | [Link](https://www.youtube.com/watch?v=IYvD9oBCuJI)React State Vs  first thing to happen in the lifecycle of React | [Link](https://blog.logrocket.com/react-lifecycle-methods-tutorial-examples/#:~:text=to%20be%20updated%3F-,1.,invoked%20during%20the%20updating%20phase.)

 