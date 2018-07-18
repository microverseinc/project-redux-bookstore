# Milestone 3

## Introduction

Alrighty! The foundation is built. Here comes the real job. In this milestone, we'll connect the `CREATE_BOOK` and `REMOVE_BOOK`
actions with the React component and make our page dynamic.

## Requirements

1. Make the `BooksForm` component stateful
    - The component should store the title and the book category in its own state.
    - The component should implement the `handleChange` method which reacts to the user typing to input a name or to changes in the category select.
    - Each change to the form should modify the component's state.
    - The component should implement `handleSubmit` which will save the new book in the Redux store and resets the component's state.
    - Documentation: [Map Dispatch to Props](https://learn.co/lessons/map-dispatch-to-props-readme)
2. Connect the `REMOVE_BOOK` action to the component
    - Add a new table column to the `BooksList` component. It should render the "Remove Book" button next to each book.
    - Implement the `handleRemoveBook` method which accepts a book as an argument and removes it from the Redux store. Don't forget to pass that method down to the `Book` component as a prop.

Great! This milestone was pretty short but added some interaction to the application. Currently, the user can add a new book with title and category or remove it from the table. In the next milestone we'll add one more action and learn how to combine reducers.
