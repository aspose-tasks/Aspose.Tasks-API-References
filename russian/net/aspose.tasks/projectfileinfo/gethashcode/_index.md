---
title: "ProjectFileInfo.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "ProjectFileInfo метод. Возвращает значение хеш‑кода для экземпляра класса ProjectFileInfo"
type: docs
weight: 60
url: /ru/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Возвращает значение хеш‑кода для экземпляра класса [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как читать информацию о файле проекта.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### См. также

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


