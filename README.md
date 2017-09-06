# 操作指引

為能正常操作以下「步驟」，請依據「事前準備」章節，備妥應安裝之軟體套件。

## 編譯及執行程式

### （1）下載專案檔案
```
$ git clone https://github.com/AlanJui/AspNetCore-DataGrid-DevExtreme
```
### （2）進入專案資料夾
```
$ cd AspNetCore-DataGrid-DevExtreme
```
### （3）安裝 Client 端用 Lib 套件
```
$ bower install
```

### （4）安裝 ASP.NET Core 套件
```
$ dotnet restore
```

### （5）編譯與組建（Build）程式
```
$ dotnet build
```

### （6）啟動程式
```
$ dotnet run
```

### （7）執行程式
使用 Web 瀏覽器，瀏覽網址： http://localhost:5000


## 事前準備

### 編譯及執行程式

 - Git
 - .NET Core SDK (參考： https://www.microsoft.com/net/core )
 - NodeJS & NPM
 - Bower

### 資料庫

 - 本範例程式需要使用「北風貿易公司」資料庫，程式執行前，請先將 Northwind.bak 資料庫備份檔案，Restore 至 MS SQL Server 中。

 - 本範例程式在 MS SQL Server 的 Connection String 設定如下：
    ```
    "data source=(local);initial catalog=Northwind;integrated security=True"
    ```

    若有需要變更，請至 /Models/NorthwindContext.cs 原始碼程式檔，進行修改。

    Connection String 所在位置，如下所示：

    ```
    protected override void OnConfiguring(DbContextOptionsBuilder options) {
        ......
    }    
    ```
### 常見 SQL Connection String 用法

#### 使用 SQL Server Express 版，伺服器身份驗證方式(Server Authentication)採用「Windows Authentication」
"data source=.\SQLEXPRESS;initial catalog=Northwind;integrated security=True"

#### 使用 SQL Server (含 Developer ) 版，伺服器身份驗證方式(Server Authentication)採用「Windows Authentication」
"data source=localhost;initial catalog=Northwind;integrated security=True"

#### 使用 SQL Server (含 Developer ) 版，伺服器身份驗證方式(Server Authentication)採用「Windows Authentication」
"data source=127.0.0.1;initial catalog=Northwind;integrated security=True"

#### 使用 SQL Server (含 Developer ) 版，伺服器身份驗證方式(Server Authentication)採用「Windows Authentication」
"data source=(local);initial catalog=Northwind;integrated security=True"

#### 使用 SQL Server (含 Developer ) 版，伺服器身份驗證方式(Server Authentication)採用「SQL Server」
"data source=192.168.66.10;initial catalog=Northwind;user id=sa;password=Passw0rd"

