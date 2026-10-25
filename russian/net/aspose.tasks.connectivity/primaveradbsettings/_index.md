---
title: "Класс PrimaveraDbSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Connectivity.PrimaveraDbSettings. Позволяет задать необходимые параметры для чтения данных проекта из базы данных Primavera"
type: docs
weight: 320
url: /ru/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Позволяет задать необходимые параметры для чтения данных проекта из базы данных Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Инициализирует новый экземпляр класса `PrimaveraDbSettings`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Получает или задает строку подключения. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Получает идентификатор проекта для чтения. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Получает или задает обратный вызов, который будет вызываться во время операций загрузки проекта. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Получает или задает экземпляр DbProviderFactory, который используется для подключения к БД. Если заданы как ProviderFactory, так и ProviderInvariantName, приоритет имеет ProviderFactory. Значение по умолчанию — null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Получает или задает инвариантное имя провайдера, которое используется для получения экземпляра класса DbProviderFactory. Значение по умолчанию — SqlClient. |

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

Показывает, как получить краткую информацию о проектах из базы данных Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### См. также

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


