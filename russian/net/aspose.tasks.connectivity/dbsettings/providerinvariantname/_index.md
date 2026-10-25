---
title: "DbSettings.ProviderInvariantName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство DbSettings. Получает или задает инвариантное имя провайдера, которое используется для получения экземпляра класса DbProviderFactory. Значение по умолчанию — SqlClient"
type: docs
weight: 40
url: /ru/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Получает или задает инвариантное имя провайдера, которое используется для получения экземпляра класса DbProviderFactory. Значение по умолчанию — SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


