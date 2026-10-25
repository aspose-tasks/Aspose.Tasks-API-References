---
title: "MpdSettings.ProjectId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MpdSettings. Получает идентификатор проекта для чтения"
type: docs
weight: 20
url: /ru/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Получает идентификатор проекта для чтения.

```csharp
public int ProjectId { get; }
```

## Примеры

Показывает, как использовать настройки MPD для управления импортом проекта из базы данных.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


