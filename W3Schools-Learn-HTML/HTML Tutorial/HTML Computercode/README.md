# HTML Computer Code Elements

HTML contains several elements for defining user input and computer code.

# HTML `<kbd>` For Keyboard Input

The HTML `<kbd>` element is used to define keyboard input. The content inside is displayed in the browser's default monospace font.

Example
Define some text as keyboard input in a document:

`<p>`Save the document by pressing `<kbd>`Ctrl + S`</kbd>` `</p>`

# HTML `<samp>` For Program Output

The HTML `<samp>` element is used to define sample output from a computer program. The content inside is displayed in the browser's default monospace font.

Example
Define some text as sample output from a computer program in a document:

`<p>`Message from my computer:`</p>`
` <p>` `<samp> `File not found.`<br>`Press F1 to continue`</samp>` `</p>`

# HTML `<code>` For Computer Code

The HTML `<code>` element is used to define a piece of computer code. The content inside is displayed in the browser's default monospace font.

Example
Define some text as computer code in a document:

`<code>`
x = 5;
y = 6;
z = x + y;
`</code>`

Notice that the `<code>` element does not preserve extra whitespace and line-breaks.

To fix this, you can put the `<code>` element inside a `<pre>` element:

### Example

`<pre>`
`<code>`
x = 5;
y = 6;
z = x + y;
`</code>`
`</pre>`

# HTML `<var>` For Variables

The HTML `<var>` element is used to define a variable in programming or in a mathematical expression. The content inside is typically displayed in italic.

### Example

Define some text as variables in a document:

`<p>`The area of a triangle is: 1/2 x `<var>b</var>` x `<var>h</var>`, where `<var>b</var>` is the base, and `<var>h</var>` is the vertical height.`</p>`

# Chapter Summary

- The `<kbd>` element defines keyboard input
- The `<samp>` element defines sample output from a computer program
- The `<code>` element defines a piece of computer code
- The `<var>` element defines a variable in programming or in a mathematical expression
- The `<pre>` element defines preformatted text
