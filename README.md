# MyReadsApp

# MyReads Project
This project is in part of Udacitys Nanodegree Wed Development requirements. This development is built on the fundamentals of REACT and implementing components to create
a dynamic application that allows a user to select books from a database and place them into three categories of reading. This project utilizes REACT and single page applications to produce the dynamics required of everyday applications.
This project required the deconstruction of the static code and then turned into component pieces. A portion of the "books" code was moved into a seperate JS file and then placed as a component itself: the BookDetail file was also a portion of the original App.JS file as for the majority of the file itself. The static information was removed and route paths and booksAPI was added to generate a dynamic UI from the backend server. Additionally; Browser Router and Link was also used in this project in addition to using ES6 modules.

## To Launch:
1. Install all dependencies by opening a terminal and using  npm install
2. Install  npm install --save escape-string-regexp
3. PLEASE NOTE: You may need to install React Router Dom: if so Install npm --save react-router-dom
4. Start the backend server with npm start
5. The project will launch on local host 3000. Type localhost:3000 into your browser.

## Credits and Resources
1. Github localStorage Parse
2. http://place-hold.it/ for the image holding for BooksAPI
3. StackOverflow
4. https://www.npmjs.com/package/react-router-dom
5. Program Practical
6. Github: CoalField
7. MoOx/storage.js -Github
8. https://www.digitalocean.com -E Targets
9. Regular expression features in ECMAScript 6 http://2ality.com/2015/07/regexp-es6.html

## About the Backend Server

To simplify your development process, we've provided a backend server for you to develop against. The provided file [`BooksAPI.js`](src/BooksAPI.js) contains the methods you will need to perform necessary operations on the backend:

* [`getAll`](#getall)
* [`update`](#update)
* [`search`](#search)

### `getAll`

Method Signature:

```js
getAll()
```

* Returns a Promise which resolves to a JSON object containing a collection of book objects.
* This collection represents the books currently in the bookshelves in your app.

### `update`

Method Signature:

```js
update(book, shelf)
```

* book: `<Object>` containing at minimum an `id` attribute
* shelf: `<String>` contains one of ["wantToRead", "currentlyReading", "read"]
* Returns a Promise which resolves to a JSON object containing the response data of the POST request

### `search`

Method Signature:

```js
search(query, maxResults)
```

* query: `<String>`
* maxResults: `<Integer>` Due to the nature of the backend server, search results are capped at 20, even if this is set higher.
* Returns a Promise which resolves to a JSON object containing a collection of book objects.
* These books do not know which shelf they are on. They are raw results only. You'll need to make sure that books have the correct state while on the search page.

## Important
The backend API uses a fixed set of cached search results and is limited to a particular set of search terms, which can be found in [SEARCH_TERMS.md](SEARCH_TERMS.md). That list of terms are the _only_ terms that will work with the backend, so don't be surprised if your searches for Basket Weaving or Bubble Wrap don't come back with any results.

## Create React App

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app). You can find more information on how to perform common tasks [here](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md).
