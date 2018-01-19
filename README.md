# mysqlhw
操作指令

以下指令是執行 CONTAINER 同時ROOT帳號以及密碼設定，大括號內名字可以自由命名

`$ docker run --name {mysqlcontainer} -e MYSQL_ROOT_PASSWORD=123 -d emilienlee/mysqlhw`

================================================================================

緊接著進入CONTAINER內

`$ docker exec -it mysqlcontainer /bin/bash`

================================================================================

在CONTAINER內用ROOT以及設定的密碼登入MYSQL

`$ mysql -uroot -p123`

================================================================================

最後在使用SQL指令查詢是否有建立資料成功即可
