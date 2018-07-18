# Milestone 2

## Introduction
Your project structure and basic dependencies are now ready. Great! Now, it is time to initialize the Redux actions, reducers and store. Additionally, we'll also define empty React components. Remember to separate presentation and container components.

This time, we'll add two container components (those which connect with the Redux store): `BooksList` and `BooksForm`
and two presentational components: `App` and `Book`.

## Requirements

1. Prepare the directory structure
    - Create a `components` directory in the `src` folder for all the presentational components.
    - Create a `containers` directory in the `src` folder for all the container components.
    - Create a `actions` directory with the `index.js` file where you'll define all the Redux actions.
    - Create a `reducers` directory with two files: `books.js` and `index.js`. The former will store the functions responsible for
     actions on Books, and the latter should combine all the reducers into one. For now, it will only combine the `books.js` reducer.
    - Documentation: [Combine Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers)
2. Implement the **App** component
    - It should only wrap `BooksList` and `BooksForm` in a `div` selector and display it.
    - Attach this component to render the function in the main `index.js` file.
3. Implement the **BooksList** component
    - It should display the books as an html table.
    - Each row should contain Book ID, title and category.
    - It should connect to the Redux store and fetch the books from the state.
4. Implement the **Book** component
    - It should accept a book object as a prop.
    - It should represent a single row in the Books table.
5. Implement the **BooksForm** component
    - It should render a very simple form for adding books. The form should contain a book title input, a select box with categories and a submit button.
    - Define a constant with a collection containing the book categories: `["Action", "Biography", "History", "Horror", "Kids", "Learning", "Sci-Fi"]`.
6. Define the Redux actions and reducers
    - Implement the `books.js` reducer with `CREATE_BOOK` and `REMOVE_BOOK` actions. Remember, your state can not be mutated!
    - Define the `CREATE_BOOK` and `REMOVE_BOOK` actions in `actions/index.js`. They should accept a `book` object as an argument.
7. Initialize the Redux store
    - Create the initial state object in `src/index.js`. It may contain just a few books with different titles and categories.
    - Each book in the initial state should have a unique ID. However, we'll cheat here and implement that functionality by using the `Math.random` function.
    - Render the `<App/>` component wrapped in `<Provider>` and pass the store down to the components.


Congratulations! Your bookstore manager should display some books in the table which are stored in the Redux store. Moreover, there is a form where the user might add another book to the store. Making that form functional is the goal of the next Milestone.
