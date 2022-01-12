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

" Set text width as 100.
the possible_keys column indicates which indexes MySQL can choose from to find the rows in the table. If the column is null there is not releven indexes the column key is very important column. The key that MySQL actually decided to use. The possible_keys, was just an indication. However, the key column is the actual eky used to retrieve the results.
