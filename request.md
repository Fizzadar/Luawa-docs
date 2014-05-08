$title=Request Data, Headers & Cookies

Access current request data. Set HTTP headers & cookies and to redirect the user between pages.


## API: Data

All API data is immutable.

+ **request.get** - table of GET data
+ **request.post** - table of POST data
+ **request.header** - table of HTTP headers
+ **request.cookie** - table of cookies
+ **request.method** - HTTP method
+ **request.hostname** - hostname set by client, with default in config
+ **request.remote_addr** - IP address of the remote client


## API: Functions

### request:redirect(url, message\_type, message\_text)

+ **url**: url to redirect to
+ **message_type**: type of message to set
+ **message_text** text of message to set

Redirects the user with optional message which under the hood basically runs `session:setMessage(type, text)`.

### request:setHeader(key, value)

+ **key**: key/name of the header to set
+ **value**: value of the header

Sets a HTTP header of key => value, returns nil.

### request:setCookie(key, value, expire, path, domain, secure, httponly)

+ **key**: key of the cookie to set
+ **value**: value of the cookie
+ **expire**: number of seconds in the future to expire relative to the current date/time
+ **path**: path of the cookie
+ **domain**: domain of the cookie
+ **secure**: enable secure-only
+ **http**: enable http-only

Sets a cookie, returns nil.

### request:deleteCookie(key)

**key**: key of the cookie to delete

Deletes the cookie, returns nil.