Luawa itself.

###luawa:setConfig( dir, file )

+ **dir**: absolute location of the app
+ **file**: name of the config file relative to dir

Sets the Luawa config up.


###luawa:run()

Runs Luawa.


### Nginx Context Variables

In use by Luawa, overwrite at your own risk!:

    ngx.ctx.response
    ngx.ctx.db
    ngx.ctx.logs
    ngx.ctx.cookies
    ngx.ctx.session_id
    ngx.ctx.data
    ngx.ctx.user
   