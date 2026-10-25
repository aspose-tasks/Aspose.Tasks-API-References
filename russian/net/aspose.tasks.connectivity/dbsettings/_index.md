---
title: "Класс DbSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Connectivity.DbSettings. Позволяет указать настройки для чтения из базы данных проекта"
type: docs
weight: 290
url: /ru/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Позволяет указать настройки для чтения из базы данных проекта.

```csharp
public abstract class DbSettings
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Получает или задает строку подключения. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Получает или задает обратный вызов, который будет вызываться во время операций загрузки проекта. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Получает или задает экземпляр DbProviderFactory, который используется для подключения к БД. Если заданы как ProviderFactory, так и ProviderInvariantName, приоритет имеет ProviderFactory. Значение по умолчанию — null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Получает или задает инвариантное имя провайдера, которое используется для получения экземпляра класса DbProviderFactory. Значение по умолчанию — SqlClient. |

## Примеры

Показывает, как прочитать проект из XML‑файла Primavera с несколькими проектами, используя имя провайдера.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Создать настройки Primavera DB, используя строку подключения и идентификатор проекта
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


