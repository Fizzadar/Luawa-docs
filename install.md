Luawa is built on top of the [lua-nginx-module](https://github.com/chaoslawful/lua-nginx-module), and as such needs a working install of Lua/LuaJIT and Nginx compiled with the module. There are additional requirements depending on the modules you wish to use:

+ **Template, session and user** require Lua-cjson
+ **Database** requires an install of MySQL to connect to

More info coming soon. Example apps: [yummymarks](https://github.com/Fizzadar/yummymarks) and [Oxypanel](http://github.com/Oxygem/Oxypanel).