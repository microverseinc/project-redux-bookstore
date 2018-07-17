# Milestone 3

## Introduction

Alrighty! The foundation is built. Here comes the real job! In this milestone, we'll connect the `CREATE_BOOK` and `REMOVE_BOOK`
actions with the React component and make our page dynamic.

## Requirements

1. Make the `BooksForm` component stateful
    - Component should store title and book category in its own state.
    - Component should implement `handleChange` method which reacts to user typing to input or changing category in select.
    - Each change in form should modify the component's state.
    - Component should implement `handleSubmit` which saves new book in Redux store and resets component's state.
    - Documentation: [Map Dispatch to Props](https://learn.co/lessons/map-dispatch-to-props-readme)
2. Connect `REMOVE_BOOK` to component
    - Add new table column to `BooksList` component. It should render the "Remove Book" button next to each book.
    - Implement `handleRemoveBook` method which accepts a book as an argument and removes it from the Redux store. Don't forget to pass that method down to the `Book` component as a prop.

Great! This milestone was pretty short but added some interaction to our application. Currently, the user can add a new book with title and category or remove it from the table. In the next milestone we'll add one more action and learn how to combine reducers.
