# Postgresql terminal

## Grant privileges
```ssh
grant CONNECT, TEMPORARY, CREATE on database my_database to my_user or my_role;
```
* `my_table`: Name database;
* `my_user`: User name;
* `my_role`: Name role;

## Grant all privileges
```
grant all privileges on database my_table to my_user or my_role;
```

## Grant in schema
```
grant all privileges on all tables in schema public to my_user or my_role;

grant all privileges on all sequences in schema public to my_user or my_role;
```

## Revoke privileges
```
revoke CONNECT, TEMPORARY, CREATE on database my_database from my_user or my_role;
```

## Revoke all privileges
```
revoke all privileges on database my_table on my_database or my_role;
```

## Revoke in schema
```
revoke all privileges on all tables in schema public from my_user or my_role;

revoke all privileges on all sequences in schema public from my_user or my_role;
```

## Import table CSV
```
COPY table_name FROM 'table.csv' DELIMITER ',' CSV HEADER;
```

## Search duplicate
```
SELECT name, COUNT(id)
FROM table
GROUP BY name
HAVING COUNT(id) > 1
ORDER BY COUNT(id);
```