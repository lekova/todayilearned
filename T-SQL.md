# T-SQL

## Tips and Tricks

Find a world in column name for all tables in DB

```SQL
SELECT * FROM INFORMATION_SCHEMA.COLUMNS where COLUMN_NAME LIKE '%name%';
```
