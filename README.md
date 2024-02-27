Try to bootstrap a basic React application using vite. Read more about vite here - https://vitejs.dev/

Create the following functionality -

-> A basic TODO application where there are two input (title and description) boxes and users can add append TODOs to a div
-> Try using the same DOM functionality we did in week 4. Don't try to use state variables in React just yet
-> Just tro to port over our original HTML/JS impelementation over to a React project

You have been given the code of a purely frontend TODO app You have to fill in the following functions -

addTodoToDom
removeTodoFromDom
updateTodoInDom
updateState
These 4 functions comprise of what it means to create a library like React. The goal is the following -

Any time the updateState function is called with a new state, the updateState function calculates the diff between newTodos and oldTodos and call addTodoToDom, removeTodoFromDom or updateState based on the calculated diff.
They id of a todo uniquely identifies it. If the title of a todo with the same id changes in two iterations, updateTodoInDom should be called for it.
The structure of the state variable looks something like this -
    const todos = [{
        title: "Go to gym",
        description: "Go to gym from 7-8PM",
        id: 1
    }]