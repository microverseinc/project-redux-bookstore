# Milestone 6

## Introduction

This milestone is optional, but it can be a great addition to your portfolio, so we recommend that you go ahead and implement it.

Your application lets you keep a list of the books that you own. However, as soon as you close the browser, all the updates will get lost. What's missing here? The backend!

In order for this to be a full application, you need to connect it with a backend that can store all the information about the books that you own. Since you are already proficient with Ruby on Rails, let's build one!

## Requirements

1. You should create a new Ruby on Rails application
2. The new application will be a simple REST API
    - If you need a refresher, take a look at the following two lessons from The Odin Project: [Lesson 1](https://www.theodinproject.com/courses/ruby-on-rails/lessons/apis-and-building-your-own), [Lesson 2](https://www.theodinproject.com/courses/ruby-on-rails/lessons/apis).
3. The API should...
    - Allow you to obtain a list of books in your library
    - Allow you to remove a book from your library
    - Allow you to add a book to your library
4. Each book should have a title, author (blank by default), and a Category
5. Your React/Redux app should make GET/POST/PUT requests to your Rails API to obtain and save data
6. In order to make things simple for now, deploy the React app and the Rails app as two separate apps
    - For a refresher, take a look at [this tutorial](http://railsapps.github.io/rails-javascript-include-external.html) included in The Odin Project. It's generic for JavaScript.
7. Here is a list of optional functionality that you can building:
    - Your app should allow the user to select the reading percentage of each book
    - The app should allow the user to manage the list of available categories
    - The app should render properly in small screens (e.g. mobile devices and tablets)
    - The app should allow the user to add comments to each book in the library
    - The app should support authentication to handle multiple users and keep the user information private
    - The app should talk to the [Goodreads API](https://www.goodreads.com/api) to let the user easily add new books
