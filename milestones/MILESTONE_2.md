# Milestone 2

## Introduction
You have got your project ready for you to work. Great! Now, it is time to initialize Redux actions, reducers and store.
Additionally we'll also define empty React components. Remember, separate presentational components from containers.

This time, we'll add two container components (those which connect with Redux store): `BooksList` and `BooksForm`
and two presentational components: `App` and `Book`.

## Requirements

1. Prepare directory structure
   - Create `components` directory in `src` folder for all presentational components.
   - Create `containers` directory in `src` folder for all container components.
   - Create `actions` directory with `index.js` file where you'll define all Redux actions.
   - Create `reducers` directory with two files: `books.js` and `index.js`. The former will store functions responsible for
     actions on Books, the latter should combine all reducers in one. For now, it will combine only `books.js` reducer.
   - Documentation: [Combine Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers)
2. Implement **App** component
   - It should only wrap `BooksList` and `BooksForm` in `div` selector and display it.
   - Attach this component to render function in main `index.js` file.
3. Implement **BooksList** component
   - It should display books as html table. Each row should contain Book ID, title and category.
   - It should connect to Redux store and fetch books from state.
4. Implement **Book** component
   - It should accept book object as prop.
   - It should represent single row in Books table.
5. Implement **BooksForm** component
   - It should render very simple form for adding books. Form should contain book title input, select box with categories and
     submit button.
   - Define constant collection with book categories: `["Action", "Biography", "History", "Horror", "Kids", "Learning", "Sci-Fi"]`.
6. Define Redux actions and reducers
   - Implement `books.js` reducer with `CREATE_BOOK` and `REMOVE_BOOK` actions. Remember, your state can not be mutated!
   - Define `CREATE_BOOK` and `REMOVE_BOOK` actions in `actions/index.js`. They should accept `book` object as an argument.
7. Initialize Redux store
   - Create initial state object in `src/index.js`, it may contain few books with different titles and categories.
   - Each book in initial state should have unique ID. However we'll cheat that functionality by using `Math.random` function.
   - Render `<App/>` component wrapped in `<Provider>` and pass store down to the components.


Congratulations! Your book store should display some books in the table which are stored in Redux store. Moreover, there is a
form where user might add another book to the store and this is in fact subject of next Milestone.
