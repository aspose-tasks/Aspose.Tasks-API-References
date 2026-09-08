---
title: "VbaProject.HelpFile"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaProject. Возвращает имя файла справки."
type: docs
weight: 40
url: /ru/net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

Получает имя файла справки

```csharp
public string HelpFile { get; }
```

## Примеры

Показывает, как читать свойства проекта VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### См. также

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


