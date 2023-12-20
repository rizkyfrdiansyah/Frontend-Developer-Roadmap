# HTML id Attribute

The HTML id attribute is used to specify a unique id for an HTML element.

You cannot have more than one element with the same id in an HTML document.

# HTML Bookmarks with ID and Links

HTML bookmarks are used to allow readers to jump to specific parts of a webpage.

Bookmarks can be useful if your page is very long.

To use a bookmark, you must first create it, and then add a link to it.

Then, when the link is clicked, the page will scroll to the location with the bookmark.

Example
First, create a bookmark with the `id` attribute:
`<h2 id="C4">Chapter 4</h2>`

Or, add a link to the bookmark ("Jump to Chapter 4"), from another page:

`<a href="html_demo.html#C4">Jump to Chapter 4</a>`

# Chapter Summary

- The `id` attribute is used to specify a unique id for an HTML element
- The value of the `id` attribute must be unique within the HTML document
- The `id` attribute is used by CSS and JavaScript to style/select a specific element
- The value of the `id` attribute is case sensitive
- The `id` attribute is also used to create HTML bookmarks
- JavaScript can access an element with a specific `id` with the `getElementById()` method
