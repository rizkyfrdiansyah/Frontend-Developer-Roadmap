# HTML Drag and Drop API

In HTML, any element can be dragged and dropped.

## Drag and Drop

Drag and drop is a very common feature. It is when you "grab" an object and drag it to a different location.

## Make an Element Draggable

First of all: To make an element draggable, set the draggable attribute to true:

`<img draggable="true">`

## What to Drag - ondragstart and setData()

Then, specify what should happen when the element is dragged.

In the example above, the `ondragstart` attribute calls a function, drag(event), that specifies what data to be dragged.

The `dataTransfer.setData()` method sets the data type and the value of the dragged data:

`function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}`
In this case, the data type is "text" and the value is the id of the draggable element ("drag1").

## Where to Drop - ondragover

The `ondragover` event specifies where the dragged data can be dropped.

By default, data/elements cannot be dropped in other elements. To allow a drop, we must prevent the default handling of the element.

This is done by calling the `event.preventDefault()` method for the ondragover event:

`event.preventDefault()`

## Do the Drop - ondrop

When the dragged data is dropped, a drop event occurs.

In the example above, the ondrop attribute calls a function, drop(event):

`function drop(ev) {
ev.preventDefault();
var data = ev.dataTransfer.getData("text");
ev.target.appendChild(document.getElementById(data));
}`

Code explained:

- Call preventDefault() to prevent the browser default handling of the data (default is open as link on drop)
- Get the dragged data with the dataTransfer.getData() method. This method will return any data that was set to the same type in the setData() method
- The dragged data is the id of the dragged element ("drag1")
- Append the dragged element into the drop element
