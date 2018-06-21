# Milestone 4

## Introduction

Magic-Books Inc. requested for one additional functionality in the application. They would like to be able to filter books in
the table by category. Do you imagine how implementation for that would look like? Yes, you'll add new presentational
component `CategoryFilter` which is going to be simple select box. In addition, we'll create new Redux action `CHANGE_FILTER`
and `filter.js` reducer.

## Requirements

1. Enhance Redux store
   - Redux store should keep information about current books filter. Name it `filter`, it can be simple string with name of the
     category. Remember to add option `All` which just removes filter from table.
   - Create `CHANGE_FILTER` action in `actions/index.js`
   - Create `filter.js` reducer which modifies `filter` in Redux store. It should default to `All`.
2. Implement `CategoryFilter` component
   - Component should render select box with filter categories.
   - Remember to merge book categories with `All` option in select box. `All` is not valid book category and shouldn't be saved
     in Redux store, although it should be a filter option.
3. Keep filter value in Redux store
   - Render `CategoryFilter` component in `BooksList`.
   - Implement `handleFilterChange` method which modifies `filter` state in Redux store. Pass it down as a prop to `CategoryFilter`.
   - Implement conditional method which decides which books should be shown in table, depending on `filter` value from Redux store.

That's it! Your application is fully functional and ready to be handed over to client. Great work :)
