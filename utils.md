A set of useful functions. Note that they are accessed using "." notation rather than ":" and use underscores for function names. This is because each function is independent and therefore `luawa.utils` does not act as a 'class'.

## API Reference

### utils.table_string(table)

+ **table**: table of data

Returns a string formatted table.


### utils.html_ents(string)

+ **string**: string to convert

Returns the string with any html entities encoded.


### utils.alpha_numerify(string)

+ **string**: string to convert

Returns the string with non-alphanumeric characters removed.


### utils.capitalize_first(string)

+ **string**: string to convert

Returns the string with the first letter capitalizes.


### utils.is_email(string)

+ **string**: string to check

Returns true or false for an email ([does it contain @](http://davidcel.is/blog/2012/09/06/stop-validating-email-addresses-with-regex/))


### utils.is_url(string)

+ **string**: string to check

Returns true or false if the string starts with http:// or https://


### utils.trim(string, chars)

+ **string**: string to convert
+ **chars**: string to trim, defaults to whitespace

Returns a string with `chars` removed from both sides.


### utils.trim_right(string)

+ **string**: string to convert
+ **chars**: string to trim, defaults to whitespace

Returns a string with `chars` removed from the right side.


### utils.trim_left(string)

+ **string**: string to convert
+ **chars**: string to trim, defaults to whitespace

Returns a string with `chars` removed from the left side.


### utils.random_string(length)

+ **length**: length of string desired

Returns a pseudorandom string of your chosen length.


### utils.digest(string)

+ **string**: string to digest

Calculates and returns a sha512 hash of the input string.


### utils.url_decode(string)

+ **string**: string to convert

Returns the string with all URL components decoded.


### utils.url_encode(string)

+ **string**: string to convert

Returns the string with all URL components encoded.


### utils.explode(string, divider)

+ **string**: string to convert
+ **divider**: string to divide at

PHP-like explode a string at every divide point.