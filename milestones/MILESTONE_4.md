# Milestone 4

## Introduction

Magic-Books Inc. requested one additional functionality to be added to the application. They would like to be able to filter books in the table by category. Do you imagine what the implementation for that would look like? Yes, you'll add a new presentational component (`CategoryFilter`) which will just be a simple select box. In addition, we'll create a new Redux action (`CHANGE_FILTER`) and a `filter.js` reducer.

## Requirements

1. Enhance the Redux store
    - The Redux store should keep information about the current books filter. Name it `filter`. It can be a simple string with the name of the category. Remember to add the option `All` which will just remove the filter from the table.
    - Create the `CHANGE_FILTER` action in `actions/index.js`
    - Create a `filter.js` reducer which modifies `filter` in the Redux store. It should default to `All`.
2. Implement the `CategoryFilter` component
    - The component should render a select box with filter categories.
    - Remember to merge the book categories with the `All` option in the select box. `All` is not a valid book category and shouldn't be saved in the Redux store, although it should be a filter option.
3. Keep the filter value in the Redux store
    - Render the `CategoryFilter` component in the `BooksList` component.
    - Implement the `handleFilterChange` method which modifies the `filter` state in the Redux store. Pass it down as a prop to `CategoryFilter`.
    - Implement a conditional method which decides which books should be shown in the table depending on the `filter` value from Redux store.

That's it! Your application is fully functional and ready to be handed over to the client. Great work :)
