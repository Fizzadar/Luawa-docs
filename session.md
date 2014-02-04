$title=Session & Messages

The session module is used to manage sessions, validate forms with csrf tokens & pass messages between redirects. Sessions are stored in a shared in-memory cache provided by the Nginx Lua module.

###session:set( key, value )

+ **key**: key to set
+ **value**: value to set (string or number)

Sets session data.


###session:get( key )

+ **key**: key to get

Returns session data or nil.


###session:delete( key )

+ **key**: key to get

Deletes session data, returns nil.


###session:getToken()

Returns an anti-csrf token. It is automatically included in template data (but _not_ with the api flag, which must be manually set).


###session:checkToken( token )

**token**: token to check against

Returns true or false.


###session:addMessage( type, text )

**type**: type of message to set (for use in templates as class, for example)
**text**: the message itself

Adds a message to the session, returns nil.


###session:getMessages()

Returns a table of messages, and clears the message list.
