
### 1. Download Database Backup / Extract: 
1. **Part 1:** [https://we.tl/t-OId1RjEYa6](https://we.tl/t-OId1RjEYa6)
2. **Part 2:** [https://we.tl/t-xxt1g79LKT](https://we.tl/t-xxt1g79LKT)

3. Unzip the `tidy-db.zip` using WinRAR.

*Install [WinRAR](https://www.win-rar.com/download.html?&L=0) if not installed.

- [Click Here to Download WinRAR](https://www.win-rar.com/fileadmin/winrar-versions/winrar/winrar-x64-700.exe)


#### Process to Extract
-  Right Click on `tidy-db.zip` select `Extract to "tidy-db\"`

---

### 2. Download and Install Compass

- [Download MongoDB Community Server Download](https://www.mongodb.com/try/download/community)

    If After installation, MongoDB is not started automatically as a Windows service use the following command in Command Prompt or PowerShell:

    ```bash
    net start MongoDB
    ```


- [2. Download MongoDB Shell](https://www.mongodb.com/try/download/shell)

- [3. MongoDB Command Line Database Tools](https://www.mongodb.com/try/download/database-tools)





After Installing All the requirements. 

Make sure `mongosh` and `mongorestore` command working properly on your terminal.


```bash
PS C:\Users\sannjayy> mongosh
Current Mongosh Log ID: 6639d06a450c47774346b798
Connecting to:          mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.2.5
Using MongoDB:          7.0.9
Using Mongosh:          2.2.5

For mongosh info see: https://docs.mongodb.com/mongodb-shell/

------
   The server generated these startup warnings when booting
   2024-05-07T12:20:53.323+05:30: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test>
```



### If it is working we are ready to migrate the data.

- Go to the downloaded database path & open terminal there.

run the following commands.

```bash
mongorestore --uri=mongodb://127.0.0.1:27017/tidypigeon tidy-db/
```

----
Open MongoDB Compass

On URI: `mongodb://localhost:27017` and click on connect.

On Right Corner You'll get your database named `tidypigeon`


---

