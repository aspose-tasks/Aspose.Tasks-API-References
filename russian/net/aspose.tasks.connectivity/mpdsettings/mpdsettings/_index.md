---
title: "MpdSettings.MpdSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор MpdSettings. Инициализирует новый экземпляр класса MpdSettings"
type: docs
weight: 10
url: /ru/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Инициализирует новый экземпляр класса [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| connectionString | Строка | указанная строка подключения. |
| projectId | Int32 | указанный идентификатор проекта для чтения. |

## Примеры

Показывает, как прочитать проект из MPD-файла.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


