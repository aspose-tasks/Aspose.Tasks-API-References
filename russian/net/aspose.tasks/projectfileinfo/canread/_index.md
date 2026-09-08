---
title: "ProjectFileInfo.CanRead"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "ProjectFileInfo свойство. Возвращает значение, указывающее, может ли Aspose.Tasks обрабатывать файл проекта"
type: docs
weight: 10
url: /ru/net/aspose.tasks/projectfileinfo/canread/
---
## ProjectFileInfo.CanRead property

Возвращает значение, указывающее, может ли Aspose.Tasks обрабатывать файл проекта.

```csharp
public bool CanRead { get; }
```

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


