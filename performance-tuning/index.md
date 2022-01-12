# index analysis
```
SHOW INDEX FROM table_name FROM db_name;
# or 
SHOW INDEX FROM table_name

# schema table also provide indexing statistics
SELECT * 
FROM INFORMATION_SCHEMA.STAtISTICS 
WHERE TABLE_NAME = table_name;

# Create index example
CREATE INDEX index_name ON table_name(column_name);

# To know whether the index is being used or not do the following command
EXPLAIN SELECT column_name_like_id, other_colomn_name_on_which_index_applied
FROM table_name
WHERE 
other_colomn_name_on_which_index_applied = value;


```

The possible_keys column indicates which indexes MySQL can choose from to find the rows in the table. If the column is null there is not releven indexes the column key is very important column. The key that MySQL actually decided to use. The possible_keys, was just an indication. However, the key column is the actual eky used to retrieve the results.

The column key_len indicates the length of the key that MySQL decided to use. 

```
# Drop index
DROP Index index_name ON table_name;

# FORCE INDEX enforce to use the index given in INDEX  parameter
EXPLAIN SELECT column1, column2
FROM table_name FORCE INDEX (index_name)
WHERE
column = ???

# USE gives MySQL suggesation to use the index
EXPLAIN SELECT column1, column2
FROM table_name USE INDEX (index_name_1,index_name_2,index_name_n) 
WHERE
column = ???

```

