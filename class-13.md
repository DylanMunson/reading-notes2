# Read: 13 - Local Storage

## Introducing HTML5 Storage

HTML5 Storage is another way of saying web storage. HTML5 storage is a way for web pages to store named key/value pairs locally within the client web browser. This data will be stored even if you close the browser completely, but unlike cookies, this data is never sent to the remote web server. This storage is implemented natively which means it will be available even when third-party plugins are not. HTML5 storage is supported on the most recent version of virtually every web browser and is almost always useable. You can access your html5 storage through the *localstorage* object.

## Using HTML5 Storage

HTML5 storage is based on key/value pairs, you store data with name key, and you can access that data using the same key, which is a string. This data can be any type that is supported by JS, but it is still stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to change your retrieved data into the expected JS datatype. Calling setItem() with a named key that already exists will silently overwrite the previous value, and calling getItem() with a non-existent key will return null. Like other JavaScript objects, you can treat the localStorage object as an array. Instead of using the getItem() and setItem() methods, you can simply use square brackets.

[Back](https://dylanmunson.github.io/reading-notes/)
