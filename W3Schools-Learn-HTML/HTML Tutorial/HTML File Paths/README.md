# HTML File Paths

A file path describes the location of a file in a web site's folder structure.

# File Path Examples

`<img src="picture.jpg">` The "picture.jpg" file is located in the same folder as the current page
`<img src="images/picture.jpg">` The "picture.jpg" file is located in the images folder in the current folder
`<img src="/images/picture.jpg">` The "picture.jpg" file is located in the images folder at the root of the current web
`<img src="../picture.jpg">` The "picture.jpg" file is located in the folder one level up from the current folder

# HTML File Paths

A file path describes the location of a file in a web site's folder structure.

File paths are used when linking to external files, like:

- Web pages
- Images
- Style sheets
- JavaScripts

# Best Practice

It is best practice to use relative file paths (if possible).

When using relative file paths, your web pages will not be bound to your current base URL. All links will work on your own computer (localhost) as well as on your current public domain and your future public domains.
