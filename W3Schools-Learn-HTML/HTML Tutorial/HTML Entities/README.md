# HTML Entities

Reserved characters in HTML must be replaced with entities:

- < (less than) = &lt;
- > (greather than) = &gt;

# HTML Character Entities

Some characters are reserved in HTML.

If you use the less than (<) or greater than (>) signs in your HTML text, the browser might mix them with tags.

Entity names or entity numbers can be used to display reserved HTML characters.

Entity names look like this:
`&entity_name;`

Entity numbers look like this:
`&#entity_number;`

To display a less than sign (<) we must write: &lt; or &#60;

# Non-breaking Space

A commonly used HTML entity is the non-breaking space: &nbsp;

A non-breaking space is a space that will not break into a new line.

Two words separated by a non-breaking space will stick together (not break into a new line). This is handy when breaking the words might be disruptive.

Examples:

- § 10
- 10 km/h
- 10 PM
  Another common use of the non-breaking space is to prevent browsers from truncating spaces in HTML pages.

If you write 10 spaces in your text, the browser will remove 9 of them. To add real spaces to your text, you can use the &nbsp; character entity.

The non-breaking hyphen (&#8209;) is used to define a hyphen character (‑) that does not break into a new line.

# Combining Diacritical Marks

A diacritical mark is a "glyph" added to a letter.

Some diacritical marks, like grave ( ̀) and acute ( ́) are called accents.

Diacritical marks can be used in combination with alphanumeric characters to produce a character that is not present in the character set (encoding) used in the page.
