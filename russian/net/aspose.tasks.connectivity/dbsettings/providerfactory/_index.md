---
title: "DbSettings.ProviderFactory"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство DbSettings. Получает или задает экземпляр DbProviderFactory, который используется для подключения к БД. Если заданы как ProviderFactory, так и ProviderInvariantName, приоритет имеет ProviderFactory. Значение по умолчанию — null."
type: docs
weight: 30
url: /ru/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Получает или задает экземпляр DbProviderFactory, который используется для подключения к БД. Если заданы как ProviderFactory, так и ProviderInvariantName, приоритет имеет ProviderFactory. Значение по умолчанию — null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## Примеры

Показывает, как импортировать проект из базы данных Primavera.

```csharp
// Инициализировать новый экземпляр класса PrimaveraDbSettings с строкой подключения и идентификатором проекта
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// прочитать проект с UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### См. также

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


