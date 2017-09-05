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

由於範例使用「北風貿易公司」的資料，請於程式執行前，先將 Northwind 資料，Restore 到 MS SQL Server 的資料庫之中。


