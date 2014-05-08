$title=Documentation

Luawa is a web application framework based on the Nginx Lua module. It provides lots of useful web-specific features as well as a lightweight user & permissions system. This documentation is a work in progress and relates to Luawa `v0.9.5`.

[Main website](http://luawa.com) & [install documentation](/install).

Luawa consists of a number of (somewhat independent) modules which form the basics of any web application:

+ **Request Data**, **Headers** & **Cookies**: [request.lua](/request)
+ **Session** management & **Messaging between requests**: [session.lua](/session)
+ **Database**: [database.lua](/database)
+ **User** registration, login/out, **permissions**: [user.lua](/user)
+ **Template** processing: [template.lua](/template)
+ **Utilities**: [utils.lua](/utils)
+ **Debug**: [debug.lua](/debug)
+ **Core** internals: [core.lua](/core)