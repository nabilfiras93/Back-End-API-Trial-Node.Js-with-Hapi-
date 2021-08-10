
## Sample hapi.js REST API

---
Start by cloning this repo and going inside the project's folder:

```shell
$ git clone git@github.com:nabilfiras93/Simple-API-Node.Js-with-Hapi.git
$ cd sample-hapi-rest-api
```


Run :

```shell
$ npm install
$ npm start
```


That's it! You should be able to play around your API GETting, POSTing, PUTing AND DELETEing Tasks. The end-points are as described in the `src/routes.js` file:

```shell
const routes = [
  {method: 'POST',path: '/books',handler: addBookHandler,
  },
  {method: 'GET',path: '/books',handler: getAllBooksHandler,
  },
  {method: 'GET',path: '/books/{bookId}',handler: getBookByIdHandler,
  },
  {method: 'PUT',path: '/books/{bookId}',handler: editBookByIdHandler,
  },
  {method: 'DELETE',path: '/books/{bookId}',handler: deleteBookByIdHandler,
  },
  {method: '*',path: '/{any*}',handler: () => 'Sorry, Page not found',
  },
];
```


## Try API (POSTMAN)
try API with POSTMAN collection