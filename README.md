# Book List Web App

This README explains the functionality of the code for a web app that displays a list of books and provides search and theme toggling features. The code is designed to be beginner-friendly and user-friendly.

## Table of Contents
- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Functionality](#functionality)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This web app allows users to view a list of books, apply search filters, and toggle between dark and light themes. It's written in JavaScript and utilizes HTML and CSS for the user interface.

## Getting Started
To get started, you need to include the necessary HTML structure in your webpage. This code assumes you have the following elements in your HTML:

```html
<div data-list-items></div> <!-- For displaying the book list -->
<div class="search-input"></div> <!-- For the search input -->
<div class="mode-button"></div> <!-- For toggling themes -->
```

Additionally, make sure to include a separate data module, such as `data.js`, which contains the data of books, authors, genres, and `BOOKS_PER_PAGE` constant.

## Functionality

### Rendering the Book List
- The `renderBookList` function is responsible for rendering a list of books on the page.
- It calculates the number of books to display per row based on the screen width and dynamically adjusts the width of book divs.
- Books are created as div elements with their images, titles, and authors.
- A click event listener is added to each book item to create a preview when clicked.
- The "Show more" button allows you to load more books by incrementing the `currentPage` and calling `renderBookList`.

### Searching for and Filtering Books
- The `searchBooks` function filters books based on provided search parameters such as title, genre, and author.
- The search parameters are obtained from the user interface elements.
- When the "Search" button is clicked, the `renderFilteredBooks` function is called to display the filtered books.

### Previewing Books
- The `createBookPreview` function creates a preview of a book when a book item is clicked.
- The preview contains the book's image, title, author, publication date, and description.
- Users can close the preview by clicking the "Close" button.

### Toggling Themes
- Users can toggle between dark and light themes using the theme button in the header.
- The `toggleTheme` function switches the CSS classes and styles to apply the selected theme.

## Usage
To use this code in your project, follow these steps:

1. Include the necessary HTML structure and elements as described in the "Getting Started" section.
2. Make sure you have the data module, e.g., `data.js`, with the required data.
3. Include the provided JavaScript code in your project.
4. Customize the app to fit your specific use case or design.

## Contributing
Contributions and improvements to this code are welcome. Feel free to fork the repository, make changes, and submit pull requests.

Please enjoy using and customizing this web app for your needs. If you have any questions or need assistance, feel free to reach out!
