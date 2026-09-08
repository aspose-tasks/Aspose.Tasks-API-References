---
title: "GetProjectUids"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Возвращает список уникальных идентификаторов проектов."
type: docs
weight: 20
url: /ru/net/aspose.tasks/primaveraxmlreader/getprojectuids/
---
## PrimaveraXmlReader.GetProjectUids method

Верните список уникальных идентификаторов проектов.

```csharp
public List<int> GetProjectUids()
```

### Возвращаемое значение

Список уникальных идентификаторов проектов.

### Примеры

Показывает, как импортировать проект из файла Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### См. также

* class [PrimaveraXmlReader](../../primaveraxmlreader)
* namespace [Aspose.Tasks](../../primaveraxmlreader)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
