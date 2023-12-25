# HTML Form Attributes

This chapter describes the different attributes for the HTML `<form>` element.

# The Target Attribute

The `target` attribute specifies where to display the response that is received after submitting the form.

The `target` attribute can have one of the following values:

`_blank` The response is displayed in a new window or tab
`_self` The response is displayed in the current window
`_parent` The response is displayed in the parent frame
`_top` The response is displayed in the full body of the window
`framename` The response is displayed in a named iframe
The default value is `_self` which means that the response will open in the current window.

### Notes on GET:

- Appends the form data to the URL, in name/value pairs
- NEVER use GET to send sensitive data! (the submitted form data is visible in the URL!)
- The length of a URL is limited (2048 characters)
- Useful for form submissions where a user wants to bookmark the result
- GET is good for non-secure data, like query strings in Google

### Notes on POST:

- Appends the form data inside the body of the HTTP request (the submitted form data is not shown in the URL)
- POST has no size limitations, and can be used to send large amounts of data.
- Form submissions with POST cannot be bookmarked

  Tip: Always use POST if the form data contains sensitive or personal information!
