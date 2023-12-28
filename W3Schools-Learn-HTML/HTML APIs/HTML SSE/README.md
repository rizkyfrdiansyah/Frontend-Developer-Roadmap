# HTML SSE API

Server-Sent Events (SSE) allow a web page to get updates from a server.

## Server-Sent Events - One Way Messaging

A server-sent event is when a web page automatically gets updates from a server.

This was also possible before, but the web page would have to ask if any updates were available. With server-sent events, the updates come automatically.

Examples: Facebook/Twitter updates, stock price updates, news feeds, sport results, etc.

## Check Server-Sent Events Support

In the tryit example above there were some extra lines of code to check browser support for server-sent events:

`if(typeof(EventSource) !== "undefined") {
  // Yes! Server-sent events support!
  // Some code.....
} else {
  // Sorry! No server-sent events support..
}`

## Server-Side Code Example

For the example above to work, you need a server capable of sending data updates (like PHP or ASP).

The server-side event stream syntax is simple. Set the "Content-Type" header to "text/event-stream". Now you can start sending event streams.

Code in PHP (demo_sse.php):
`<?php
header('Content-Type: text/event-stream');
header('Cache-Control: no-cache');`

`$time = date('r');
echo "data: The server time is: {$time}\n\n";
flush();
?>`

Code in ASP (VB) (demo_sse.asp):

`<%
Response.ContentType = "text/event-stream"
Response.Expires = -1
Response.Write("data: The server time is: " & now())
Response.Flush()
%>`

Code explained:

- Set the "Content-Type" header to "text/event-stream"
- Specify that the page should not cache
- Output the data to send (Always start with "data: ")
- Flush the output data back to the web page

## The EventSource Object

In the examples above we used the onmessage event to get messages. But other events are also available:

- onopen When a connection to the server is opened
- onmessage When a message is received
- onerror When an error occurs
