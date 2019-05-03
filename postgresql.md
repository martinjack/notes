# Postgresql terminal

## Grant privileges
```ssh
grant CONNECT, TEMPORARY, CREATE on database my_database to my_user or my_role;
```
`my_table`: Name database;
`my_user`: User name;
`my_role`: Name role;
## Grant all privileges
```
grant all privileges on database my_table to my_user or my_role;
```
## Revoke privileges
```
revoke CONNECT, TEMPORARY, CREATE on database my_database from my_user or my_role;
```
## Revoke all privileges
```
revoke all privileges on database my_table on my_database or my_role;
```