# HTML Versus XHTML

XHTML is a stricter, more XML-based version of HTML.

# What is XHTML?

- XHTML stands for EXtensible HyperText Markup Language
- XHTML is a stricter, more XML-based version of HTML
- XHTML is HTML defined as an XML application
- XHTML is supported by all major browsers

# Why XHTML?

XML is a markup language where all documents must be marked up correctly (be "well-formed").

XHTML was developed to make HTML more extensible and flexible to work with other data formats (such as XML). In addition, browsers ignore errors in HTML pages, and try to display the website even if it has some errors in the markup. So XHTML comes with a much stricter error handling.

If you want to study XML, please read our XML Tutorial.

# The Most Important Differences from HTML

- `<!DOCTYPE>` is mandatory
- The xmlns attribute in `<html>` is mandatory
- `<html>, <head>, <title>, and <body>` are mandatory
- Elements must always be properly nested
- Elements must always be closed
- Elements must always be in lowercase
- Attribute names must always be in lowercase
- Attribute values must always be quoted
- Attribute minimization is forbidden

# XHTML Elements Must be Properly Nested

In XHTML, elements must always be properly nested within each other, like this:

## Correct:

`<b><i>Some text</i></b>`

## Wrong:

`<b><i>Some text</b></i>`

# XHTML Elements Must Always be Closed

In XHTML, elements must always be closed, like this:

## Correct:

`<p>This is a paragraph</p>`
`<p>This is another paragraph</p>`

## Wrong:

`<p>`This is a paragraph
`<p>`This is another paragraph

# XHTML Empty Elements Must Always be Closed

In XHTML, empty elements must always be closed, like this:

## Correct:

A break: `<br />`
A horizontal rule: `<hr />`
An image: `<img src="happy.gif" alt="Happy face" />`

## Wrong:

A break: `<br>`
A horizontal rule: `<hr>`
An image: `<img src="happy.gif" alt="Happy face">`

# XHTML Elements Must be in Lowercase

In XHTML, element names must always be in lowercase, like this:

## Correct:

`<body>`
`<p>This is a paragraph</p>`
`</body>`

## Wrong:

`<BODY>`
`<P>This is a paragraph</P>`
`</BODY>`

# XHTML Attribute Names Must be in Lowercase

In XHTML, attribute names must always be in lowercase, like this:

## Correct:

`<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>`

## Wrong:

`<a HREF="https://www.w3schools.com/html/">Visit our HTML tutorial</a>`

# XHTML Attribute Values Must be Quoted

In XHTML, attribute values must always be quoted, like this:

## Correct:

`<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>`

## Wrong:

`<a href=https://www.w3schools.com/html/>Visit our HTML tutorial</a>`

# XHTML Attribute Minimization is Forbidden

In XHTML, attribute minimization is forbidden:

## Correct:

`<input type="checkbox" name="vehicle" value="car" checked="checked" />`
`<input type="text" name="lastname" disabled="disabled" />`

## Wrong:

`<input type="checkbox" name="vehicle" value="car" checked />`
`<input type="text" name="lastname" disabled />`
