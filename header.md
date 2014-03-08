Use the headers module to set HTTP headers & cookies and to redirect the user between pages.

###header:redirect( url, message\_type, message\_text )

+ **url**: url to redirect to
+ **message_type**: type of message to set
+ **message_text** text of message to set

Redirects the user with optional message which under the hood basically runs `session:setMessage( type, text )`.


###header:setHeader( key, value )

+ **key**: key/name of the header to set
+ **value**: value of the header

Sets a HTTP header of key => value, returns nil.


###header:getHeader( key )

+ **key**: key of the header to get

Returns the relevant header or nil.


###header:getHeaders()

Returns a table of all headers.


###header:setCookie( key, value, expire, path, domain, secure, httponly )

+ **key**: key of the cookie to set
+ **value**: value of the cookie
+ **expire**: number of seconds in the future to expire relative to the current date/time
+ **path**: path of the cookie
+ **domain**: domain of the cookie
+ **secure**: enable secure-only
+ **http**: enable http-only

Sets a cookie, returns nil.


###header:getCookie( key )

**key**: key of the cookie to get

Returns the relevant cookie or nil.


###header:getCookies()

Returns a table of all the cookies.


###header:deleteCookie( key )

**key**: key of the cookie to delete

Deletes the cookie, returns nil.