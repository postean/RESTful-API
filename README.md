# RESTful-API

Создание собственного веб-API RESTful с помощью ASP.NET Core и Entity Framework Core (.NET 6) с автоматическим заполнением данных в MS SQL.

Для создания  этого проекта вам понадобится следующее:

Visual Studio IDE или аналогичный
Microsoft SQL Express с SQL Server Management Studio
Пакет SDK для .NET 6 

База данных создана с использованием подхода EF Core Code-First, а данные заполнены приложением.  Использован SQL Server Management Studio (SSMS) для проверки того, что данные были перенесены и заполнены приложением.

Перенос и обновление базы данных с демонстрационными данными:
Для миграции, установлен один дополнительный пакет/зависимость. Он называется Microsoft.EntityFrameworkCore.Design и необходим для работы основных инструментов Entity Framework. 
выполнена следующая команда в терминале:

$ dotnet ef migrations add initial

Это создаст новую папку Migrationsс именем файла миграции и моментальным снимком AppDbcontext.
Для обновления  базы данных выполнена следующая команда в терминале:

$ dotnet ef database update

тестировать конечные точки можно с помощью Swagger, но вы можете использовать любой инструмент, который вы предпочитаете, например postman.

Get all Authors /api/Author
Get single Author /api/Author/id
Add new Author
Update Author /api/Author/id
Delete Author




