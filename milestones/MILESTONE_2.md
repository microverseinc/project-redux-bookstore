# Milestone 2

## Introduction
You got your project ready for you to work. Great! Now, it is time to initialize the Redux actions, reducers and store.
Additionally, we'll also define empty React components. Remember, separate presentation and container components.

This time, we'll add two container components (those which connect with the Redux store): `BooksList` and `BooksForm`
and two presentational components: `App` and `Book`.

## Requirements

1. Prepare directory structure
   - Create `components` directory in `src` folder for all presentational components.
   - Create `containers` directory in `src` folder for all container components.
   - Create `actions` directory with `index.js` file where you'll define all Redux actions.
   - Create `reducers` directory with two files: `books.js` and `index.js`. The former will store functions responsible for
     actions on Books, the latter should combine all reducers into one. For now, it will only combine the `books.js` reducer.
   - Documentation: [Combine Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers)
2. Implement **App** component
   - It should only wrap `BooksList` and `BooksForm` in `div` selector and display it.
   - Attach this component to render the function in the main `index.js` file.
3. Implement **BooksList** component
   - It should display books as an html table.
   - Each row should contain Book ID, title and category.
   - It should connect to Redux store and fetch books from state.
4. Implement **Book** component
   - It should accept a book object as prop.
   - It should represent a single row in the Books table.
5. Implement **BooksForm** component
   - It should render a very simple form for adding books. The form should contain a book title input, a select box with categories and a submit button.
   - Define constant collection with book categories: `["Action", "Biography", "History", "Horror", "Kids", "Learning", "Sci-Fi"]`.
6. Define Redux actions and reducers
   - Implement `books.js` reducer with `CREATE_BOOK` and `REMOVE_BOOK` actions. Remember, your state can not be mutated!
   - Define `CREATE_BOOK` and `REMOVE_BOOK` actions in `actions/index.js`. They should accept `book` object as an argument.
7. Initialize Redux store
   - Create the initial state object in `src/index.js`. It may contain just a few books with different titles and categories.
   - Each book in the initial state should have a unique ID. However we'll cheat that functionality by using the `Math.random` function.
   - Render `<App/>` component wrapped in `<Provider>` and pass the store down to the components.


Congratulations! Your book store should display some books in the table which are stored in Redux store. Moreover, there is a
form where user might add another book to the store and this is in fact the subject of the next Milestone.
