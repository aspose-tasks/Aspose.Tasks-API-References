---
title: "Класс PrimaveraXmlReader"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.PrimaveraXmlReader. Представляет считыватель, который позволяет извлекать UID проектов из файла Primavera Xml"
type: docs
weight: 1400
url: /ru/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Представляет считыватель, который позволяет получать UID проектов из файла Primavera Xml.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Инициализирует новый экземпляр класса `PrimaveraXmlReader`. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Инициализирует новый экземпляр класса `PrimaveraXmlReader`. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Возвращает список объектов с краткой информацией о проекте. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Верните список уникальных идентификаторов проектов. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Загружает проект с указанным уникальным идентификатором. |

## Примеры

Показывает, как просмотреть информацию о коротких проектах из файла Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### См. также

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


