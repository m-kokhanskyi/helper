
Перегляд користувачів

`SELECT host, user, authentication_string FROM mysql.user;`

Update host-user

`UPDATE mysql.user SET host = '10.10.10.10' WHERE host = 'localhost' AND user = 'root';`

Перегляд прав

`SHOW GRANTS FOR 'root'@'localhost';`

Права на перегляд і редагування. Не дозволено видаляти ні таблиці ні записи

`GRANT SELECT,UPDATE,INSERT,CREATE,ALTER,INDEX,EVENT,TRIGGER,LOCK TABLES,REFERENCES ON database . * TO 'root'@'localhost';`
