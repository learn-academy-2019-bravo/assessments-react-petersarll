# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs) -
true. however you can make multi page applications in react as well.

- React is a modern, efficient answer to complex UI applications
true

- React is a full stack framework for modern web applications
false.

- React is a flexible library that plays the role of V in an MVC framework
true

 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.

 //Your Answer
dumb components basically just present information. the components themselves really only need a render method and dont have state to worry about.  while smart components will keep track of state. They will be changing information.

 //Googled Answer
 "Smart components (or container components) on the other hand have a different responsibility. Because they have the burden of being smart, they are the ones that keep track of state and care about how the app works."
 "Dumb components are also called ‘presentational’ components because their only responsibility is to present something to the DOM. Once that is done, the component is done with it. No keeping tabs on it, no checking in once in a while to see how things are going. Nope. Put the info on the page and move on."

#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?


 //Your Answer
 yarn add will add the packages necessary to open your file in react JS. depending on what you want to add as well, you can add bootstrap or other frameworks

 //Googled Answer
"adding dependencies. when you want to use another package, you first need to add it to your dependencies. this means running yarn add [package-name] to install it into your project. This will also update your package.json and your yarn.lock so that other developers working on the project will get the same dependencies as you when they run yarn or yarn install.""

Most packages will be installed from the npm registry and referred to by simply their package name. For example, yarn add react will install the react package from the npm registry. "


#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:

    import React, { Component } from 'react';

    class Recipes extends Component {
      constructor(props){
        super(props)
        this.state = {
          recipes:
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}

        }
      }

      render() {
          let recipes = this.state.recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })
        return (

            <div>
                <ul>
                {recipes}
                </ul>
            </div>      
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)

 //Your Answer
text, submit, image, color

 //Googled Answer
 <input type="button">
 <input type="checkbox">
 <input type="color">
 <input type="date">
 <input type="datetime-local">
 <input type="email">
 <input type="file">
 <input type="hidden">
 <input type="image">
 <input type="month">
 <input type="number">
 <input type="password">
 <input type="radio">
 <input type="range">
 <input type="reset">
 <input type="search">
 <input type="submit">
 <input type="tel">
 <input type="text">
 <input type="time">
 <input type="url">
 <input type="week">



 #### 7. How would you explain state to a friend who doesn't know code?

 //Your Answer
this state = is immutable, meaning it does not change. basically a value that will stay the same.
this setState is a value that you are allowing to change. so you have the same value as you did in this state but now you are setting (changing) the value as you see fit. you are setting the stage now! you can change it to whatever you want.  


 //Googled Answer
State is like a data store to the ReactJS component. It is mostly used to update the component when user performed some action like clicking button, typing some text, pressing some key, etc.

 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.


 //Your Answer
states are basically used to store data on your current page while props pass down date to your child component.



 //Googled Answer
 What does “props” even mean?

 To get the jargon out of the way, “props” is short for “properties” so nothing particularly fancy there.

 Well, all right then. What makes props special?

 props are passed into the component

 Like props, state holds information about the component. However, the kind of information and how it is handled is different.

By default, a component has no state. The Welcome component from above is stateless:



#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.

I think building the tic tac toe was by far the best experience. It went from thinking we were going to have a very difficult time building it, to becoming one of the most enjoyable creations to date.

I think one of the most frustrating things about coding is that sometimes you just dont feel like you understand it, and then after an hour or two of trying to figure it out, you just understand it and it clicks. being able to stay in the game, be focused and keep pushing through is so important.

I think pair programming is so important with coding because youre able to bounce ideas off of one another and even if you do get stuck, you can talk to each other, slow down and push through it. having smeone that can pull you back to reality is so important.
