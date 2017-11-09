# Errors

<aside class="notice">Certain new developer features are not supported on the legacy A28 platform</aside>

The Linkplay Mobile SDK functions produce the following common error codes:


Error Code | Meaning
---------- | -------
400 | Bad Request -- Your request sucks.
401 | Unauthorized -- The device is not logged to make this particular action.
403 | Forbidden -- The requested is hidden for administrators only.
404 | Not Found -- The specified request could not be found.
405 | Method Not Allowed -- You tried to access the device with an method invalid for that platform.
406 | Not Acceptable -- You requested a format that isn't json.
500 | Internal Server Error -- Connection between device and server is unstable. Try again later.
503 | Service Unavailable -- Device is offline. Please try again later.
