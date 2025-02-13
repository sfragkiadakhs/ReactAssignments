# Getting Started with book-library

The purpose of this application is to present the most common use-cases of using the React Router.

These cases include:

- setting dynamic parameters in a url and handle them accordingly.
- using a Private Route to render Components, accourding to the user's identity.
- setting a 404 Not Found for urls that are out of our application's responsibility.

Our context is fetched from the /public/books.json, a file containing data about the id, the title, the author and the description of som books.

<U>Available Routes.</u>

- On http://localhost:3000/ the <Books> component renders, containg each book's title and author that fetched from the books.json.\
  If the url contains a URLSearchParams(for example: http://localhost:3000?search=ApPle) we check if the query parameter is "search", and then present the titles that are relevant to the search specified search parameter. We filter out each book's matching title with the search parameter in a case-insensitive way.(In our example titles with the word apple will be shown).
  Note: URLSearchParams works only when requesting the http://localhost:3000/.

- The http://localhost:3000/books redirects the user to the http://localhost:3000/,

- The http://localhost:3000/books/x will show data depending the existense of a book with id x. These data include title, author and the book's description.

- The http://localhost:3000/secret if the isAuthenticated of the component PrivateRoute is set to true will render the <SecretBooks> component with the books that an authorized user should view, otherwise redirects the user to the http://localhost:3000. The purpose of this assignment is to understand the case, thats why we dont use a backend example, but a simple mock variable.

- Every other route that is not described above, will render the <NotFound> Component.

## Available Scripts

In the project directory, you can run:

### `npm install`

Installs the dependencies to run this project.

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.
