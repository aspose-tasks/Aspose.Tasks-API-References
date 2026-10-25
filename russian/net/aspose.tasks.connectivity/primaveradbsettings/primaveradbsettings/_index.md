---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PrimaveraDbSettings. Инициализирует новый экземпляр класса PrimaveraDbSettings."
type: docs
weight: 10
url: /ru/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Инициализирует новый экземпляр класса [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connectionString | Строка | указанная строка подключения. |
| projectId | Int32 | указанный идентификатор проекта для чтения. |

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


