Luawa itself.

## Nginx Context Variables

Luawa uses a number of [Nginx ctx variables internally](https://github.com/openresty/lua-nginx-module#ngxctx), overwrite at your own risk!:

    ngx.ctx.response -- core.lua
    ngx.ctx.db -- database.lua
    ngx.ctx.logs -- debug.lua
    ngx.ctx.stack -- debug.lua
    ngx.ctx.cookies -- request.lua
    ngx.ctx.new_cookies -- request.lua
    ngx.ctx.session_id -- session.lua
    ngx.ctx.data -- template.lua
    ngx.ctx.user -- user.lua


## API Reference

### luawa:setConfig(root, file)

+ **file**: name of the config file relative to dir

Sets the Luawa config up.


### luawa:run()

Runs Luawa.


### luawa:prepareRequest()

### luawa:endRequest(error, url)

### luawa:redirect(url)

### luawa:error(type, message)

### luawa:exit(object)

### luawa:processFile(file)

### luawa:processFunction(func, file)
