---
title: "Класс PrimaveraXerReader"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.PrimaveraXerReader. Представляет считыватель для чтения UID проекта из файла Primavera XER"
type: docs
weight: 1390
url: /ru/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Представляет считыватель для чтения UID проектов из файла Primavera XER

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Инициализирует новый экземпляр класса `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Инициализирует новый экземпляр класса `PrimaveraXerReader`. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Возвращает список объектов с краткой информацией о проекте. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Верните список уникальных идентификаторов проектов. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Загружает проект с указанным уникальным идентификатором. |

## Примеры

Показывает, как просмотреть информацию о кратких проектах из файла Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### См. также

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


