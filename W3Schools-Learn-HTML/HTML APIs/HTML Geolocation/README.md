# HTML Geolocation API

The HTML Geolocation API is used to locate a user's position.

## Locate the User's Position

The HTML Geolocation API is used to get the geographical position of a user.

Since this can compromise privacy, the position is not available unless the user approves it.

### Example explained:

- Check if Geolocation is supported
- If supported, run the getCurrentPosition() method. - If not, display a message to the user
- If the getCurrentPosition() method is successful, it returns a coordinates object to the function specified in the parameter (showPosition)
- The showPosition() function outputs the Latitude and Longitude
  The example above is a very basic Geolocation script, with no error handling.

## Location-specific Information

This page has demonstrated how to show a user's position on a map.

Geolocation is also very useful for location-specific information, like:

Up-to-date local information
Showing Points-of-interest near the user
Turn-by-turn navigation (GPS)

## The getCurrentPosition() Method - Return Data

The getCurrentPosition() method returns an object on success. The latitude, longitude and accuracy properties are always returned. The other properties are returned if available:

- `coords.latitude` The latitude as a decimal number (always returned)
- `coords.longitude` The longitude as a decimal number (always returned)
- `coords.accuracy` The accuracy of position (always returned)
- `coords.altitude` The altitude in meters above the mean sea level (returned if available)
- `coords.altitudeAccuracy` The altitude accuracy of position (returned if available)
- `coords.heading` The heading as degrees clockwise from North (returned if available)
- `coords.speed` The speed in meters per second (returned if available)
- `timestamp` The date/time of the response (returned if available)
