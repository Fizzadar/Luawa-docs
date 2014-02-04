The user module provides a full user registration, login and logout system. There are helper functions to reset passwords via email and check against group based permissions lists as well. When logged in the user module represents the currently logged in user.

###user:resetPassword( email )

+ **email**: email of the user in question

Returns `key/false, possible_error` where key is the key to validate this user, which your app should email to them.


###user:resetPasswordLogin( email, key )

+ **email**: email of the user
+ **key**: reset key

Logs in a user using their email and a reset key, see `user:resetPassword`


###user:register( email, password, name )

+ **email**: email of the new user
+ **password**: password of the new user
+ **name**: username of the new user

Returns `true/false, possible_error`.


###user:login( email, password, hashed )

+ **email**: email of the user
+ **password**: password to check against
+ **hashed**: if true we don't hash the password (clientside hashing in JS, for example)

Returns true/false.


###user:logout()

Logs out the current user if any, returns nil.


###user:checkLogin()

Checks if a user is logged in, returns true/false.


###user:checkPermission( permission )

+ **permission**: name of the permission

Checks for a permission against the current user & their group, returns true/false.


###user:getData()

Returns the current users data as a table or `false, error`.


###user:setData( table:fields )

Sets the current users data. Returns true or `false, error`.