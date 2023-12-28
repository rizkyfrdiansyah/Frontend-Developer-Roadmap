# HTML Web Storage API

HTML web storage; better than cookies.

## What is HTML Web Storage?

With web storage, web applications can store data locally within the user's browser.

Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.

Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.

Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.

## HTML Web Storage Objects

HTML web storage provides two objects for storing data on the client:

- `window.localStorage` - stores data with no expiration date
- `window.sessionStorage` - stores data for one session (data is lost when the browser tab is closed)
  Before using web storage, check browser support for localStorage and sessionStorage:

`if (typeof(Storage) !== "undefined") {
// Code for localStorage/sessionStorage.
} else {
// Sorry! No Web Storage support..
}`
