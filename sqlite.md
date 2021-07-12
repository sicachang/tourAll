# sqlite3_tour

# 進入sqlite3環境 (以 `digital.db` 為例)
```cmd
sqlite3.exe digital.db
```

# 執行sql腳本 
- 以 建立`資服業`資料表 `createTable_Information_service.sql` 為例)
```cmd
sqlite3.exe digital.db ".read createTable_Information_service.sql"
```
- 以 建立`餐飲業`資料表 `createTable_Catering.sql` 為例)
```cmd
sqlite3.exe digital.db ".read createTable_Caterin.sql"
```
- 以 建立`製造業` 資料表 createTable_manufacture.sql.sql` 為例)
```cmd
sqlite3.exe digital.db ".read createTable_manufacture.sql.sql"
```

# dbToCSV (以 `digital.db` `資服業` 資料表匯出CSV 為例)

# 進入sqlite3環境 
```cmd
.headers on
.mode csv
.output information_service.csv
select * from _資服業;
.quit
```

# (線上工具)
- csvToSQL
https://blog.pulipuli.info/2017/11/csv-to-sql-tablecsv-import-csv-file.html#postcatacsv-to-sql-tablecsv-import-csv-file.html0_anchor1 

# sqllite 操控介面(db browser)
https://sqlitebrowser.org/dl/ 
- 安裝 
```cmd
next -> I accept.. -> choose both two iterm in left side (SQLite) -> next -> install 
```
- 運行 
```cmd
from start memu -> search `DB Browser`-> run 
```
- 開啟資料庫
```cmd
菜單-> 打開資料庫 -> 選擇DB (如：D:\sqlite3\digital.db) 
```

- 移除資料表(測試時誤新增之資料表)
```cmd
資料表點右鍵(如：_i1)-> 刪除資料表
```

- 查詢資料表(如：查詢`_資服業 `資料表)
-- 點選執行SQL -> 貼上 ->  `F5` 運行

```sql
select * from _資服業;
```

- 查詢資料表(如：查詢`_資服業 `資料表)
-- 點選執行SQL -> 貼上 ->  `F5` 運行

```sql
select * from _資服業;
```

```sql
select a11 from _資服業; 
```
