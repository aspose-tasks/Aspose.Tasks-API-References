---
title: "ProjectFileInfo.ProjectFileFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "ProjectFileInfo свойство. Возвращает формат файла проекта"
type: docs
weight: 40
url: /ru/net/aspose.tasks/projectfileinfo/projectfileformat/
---
## ProjectFileInfo.ProjectFileFormat property

Возвращает формат файла проекта.

```csharp
public FileFormat ProjectFileFormat { get; }
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

* enum [FileFormat](../../fileformat/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


