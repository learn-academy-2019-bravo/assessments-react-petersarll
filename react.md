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


 //Googled Answer


 #### 7. How would you explain state to a friend who doesn't know code?

 //Your Answer


 //Googled Answer


 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.


 //Your Answer


 //Googled Answer


#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
