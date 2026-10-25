---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод PrimaveraBaseReader. Возвращает список уникальных идентификаторов проектов"
type: docs
weight: 20
url: /ru/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

Верните список уникальных идентификаторов проектов.

```csharp
public List<int> GetProjectUids()
```

### Возвращаемое значение

Список уникальных идентификаторов проектов.

## Примеры

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

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


