A set of useful functions. Note that they are accessed using "." notation rather than ":" (as they are all independant).

###utils.tableString( table )

+ **table**: table of data

Returns a string formatted table.


###utils.htmlEnts( string )

+ **string**: string to convert

Returns the string with any html entities encoded.


###utils.alphaNumerify( string )

+ **string**: string to convert

Returns the string with non-alphanumeric characters removed.


###utils.capitalizeFirst( string )

+ **string**: string to convert

Returns the string with the first letter capitalizes.


###utils.isEmail( string )

+ **string**: string to check

Returns true or false for an email ([does it contain @](http://davidcel.is/blog/2012/09/06/stop-validating-email-addresses-with-regex/))


###utils.isUrl( string )

+ **string**: string to check

Returns true or false if the string starts with http:// or https://


###utils.trim( string, chars )

+ **string**: string to convert
+ **chars**: string to trim, defaults to whitespace

Returns a string with `chars` removed from both sides.


###utils.trimRight( string )

+ **string**: string to convert
+ **chars**: string to trim, defaults to whitespace

Returns a string with `chars` removed from the right side.


###utils.trimLeft( string )

+ **string**: string to convert
+ **chars**: string to trim, defaults to whitespace

Returns a string with `chars` removed from the left side.


###utils.randomString( length )

+ **length**: length of string desired

Returns a pseudorandom string of your chosen length.


###utils.digest( string )

+ **string**: string to digest

Calculates and returns a sha512 hash of the input string.


###utils.urlDecode( string )

+ **string**: string to convert

Returns the string with all URL components decoded.


###utils.urlEncode( string )

+ **string**: string to convert

Returns the string with all URL components encoded.


###utils.explode( string, divide )

+ **string**: string to convert
+ **divide**: string to divide at

PHP-like explode a string at every divide point.