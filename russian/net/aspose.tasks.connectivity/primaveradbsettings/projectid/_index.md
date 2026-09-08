---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraDbSettings. Получает идентификатор проекта для чтения."
type: docs
weight: 20
url: /ru/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Получает идентификатор проекта для чтения.

```csharp
public int ProjectId { get; }
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

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


