---
title: "ProjectFileInfo.ProjectApplicationInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ProjectFileInfo. Получает информацию о приложении файла проекта"
type: docs
weight: 30
url: /ru/net/aspose.tasks/projectfileinfo/projectapplicationinfo/
---
## ProjectFileInfo.ProjectApplicationInfo property

Возвращает информацию о приложении файла проекта.

```csharp
public ApplicationInfo ProjectApplicationInfo { get; }
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

* enum [ApplicationInfo](../../applicationinfo/)
* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


