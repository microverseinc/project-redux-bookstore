# Milestone 3

## Introduction

Alrighty! Foundation is built. Here comes the job for real men! In this milestone we'll connect `CREATE_BOOK` and `REMOVE_BOOK`
actions with React component and make our page dynamic. 

## Requirements

1. Stateful `BooksForm` component
   - Component should store title and book category in its own state.
   - Component should implement `handleChange` method which reacts to user typing to input or changing category in select.
   - Each change in form should modify component's state.
   - Component should implement `handleSubmit` which saves new book in Redux store and resets component's state.
   - Documentation: [Map Dispatch to Props](https://learn.co/lessons/map-dispatch-to-props-readme)
2. Connect `REMOVE_BOOK` to component
   - Add new table column to `BooksList` component. It should render "Remove Book" button next to each book.
   - Implement `handleRemoveBook` method which accepts book as argument and removes it from Redux store. Don't forget to pass
     that method down to `Book` component as a prop.

Great! This milestone was pretty short but added some interaction to our application. Currently user can add new book with title
and category or remove it from the table. In the next milestone we'll add one more action and learn how to combine reducers.
