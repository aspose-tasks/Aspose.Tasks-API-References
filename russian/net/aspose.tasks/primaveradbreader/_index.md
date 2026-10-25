---
title: "Класс PrimaveraDbReader"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.PrimaveraDbReader. Представляет средство чтения информации о проекте из базы данных Primavera."
type: docs
weight: 1350
url: /ru/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Представляет считыватель для чтения информации о проекте из базы данных Primavera

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Инициализирует новый экземпляр класса [`PrimaveraXerReader`](../primaveraxerreader/). |

## Методы

| Имя | Описание |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Возвращает список объектов с краткой информацией о проекте. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Верните список уникальных идентификаторов проектов. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Загружает проект с указанным уникальным идентификатором. |

## Примеры

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

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


