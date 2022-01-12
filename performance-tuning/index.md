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

```