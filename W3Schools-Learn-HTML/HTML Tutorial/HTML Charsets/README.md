# HTML Encoding (Character Sets)

To display an HTML page correctly, a web browser must know which character set to use.

# The HTML charset Attribute

The character set is specified in the <meta> tag:

### Example

`<meta charset="UTF-8">`
The HTML5 specification encourages web developers to use the UTF-8 character set.

UTF-8 covers almost all of the characters and symbols in the world!

# The ASCII Character Set

ASCII was the first character encoding standard for the web. It defined 128 different characters that could be used on the internet:

- English letters (A-Z)
- Numbers (0-9)
- Special characters like ! $ + - ( ) @ < >.

# The ANSI Character Set

ANSI (Windows-1252) was the original Windows character set:

- Identical to ASCII for the first 127 characters
- Special characters from 128 to 159
- Identical to UTF-8 from 160 to 255

  `<meta charset="Windows-1252">`

# The ISO-8859-1 Character Set

ISO-8859-1 was the default character set for HTML 4. This character set supported 256 different character codes. HTML 4 also supported UTF-8.

- Identical to ASCII for the first 127 characters
- Does not use the characters from 128 to 159
- Identical to ANSI and UTF-8 from 160 to 255

## HTML 4 Example

`<meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1">`

## HTML 5 Example

`<meta charset="ISO-8859-1">`

# The UTF-8 Character Set

- is identical to ASCII for the values from 0 to 127
- Does not use the characters from 128 to 159
- Identical to ANSI and 8859-1 from 160 to 255
- Continues from the value 256 to 10 000 characters

`<meta charset="UTF-8">`
