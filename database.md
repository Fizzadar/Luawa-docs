The database module only works with MySQL at this time. Eventually I would like to move-to/offer-alongside PostgreSQL.

All these functions (except escape) return in the format `table, error`.

+ **table**: fetched rows or has `.insert_id` or `.affected_rows`
+ **error**: string if error or nil


###database:select( table, fields, wheres, options )

+ **table**: name of table
+ **fields**: array of fields to select (non-table values select all)
+ **wheres**: table of `field = match`, sub-tables matched with `OR`
+ **options**: optional table with:
	- **limit**: number
	- **offset** = number
	- **order** (as string eg `id DESC`)
	- **group** (for `GROUP BY`)


###database:delete( table, wheres )

+ **table**: name of table
+ **wheres**: table of `field = match`, sub-tables matched with `OR`


###database:update( table, values, wheres )

+ **table**: name of table
+ **values**: table of `field = new_value`
+ **wheres**: table of `field = match`, sub-tables matched with `OR`


###datbase:insert( table, fields, values, options )

+ **table**: name of table
+ **fields**: array of fields to insert
+ **values**: table of arrays with values in matching order to fields
+ **options**: optional table with:
	- **replace**: true/false
	- **delayed**: true/false


###database:search( table, search\_fields, fetch\_fields, query )

Not currently implemented!


###database:query( sql )

+ **sql**: SQL string

Runs the SQL query.


###database:escape( data )

+ **data**: table of data

**Returns**: safe table of data to be used as insert values or where clauses.
