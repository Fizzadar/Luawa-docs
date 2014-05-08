The template module can allow you to combine Lua with HTML to form [.lhtml pages](/lhtml).

## Configuration

`config.template` options:

+ `config.template.minimize` - currently broken! Will/should automatically minimize html


## API Reference

### template:set(key, value, api)

+ **key**: key of data to set
+ **value**: value of data
+ **api**: true/false show data in API response

Sets template data.


### template:add(key, values, api)

+ **key**: key of existing data (must be table)
+ **values**: table of data to add
+ **api**: true/false show in API

Adds values to a template data table.


### template:get(key)

+ **key**: key of the data to return

Returns table data.


### template:clear()

Clears table data.


### template:put(content)

+ **content**: content to write

Writes content out in-place.


### template:load(file)

+ **file**: name of file

Load a template file and write to output.