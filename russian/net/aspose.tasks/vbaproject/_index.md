---
title: "Класс VbaProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.VbaProject. Представляет VbaProject."
type: docs
weight: 2860
url: /ru/net/aspose.tasks/vbaproject/
---
## VbaProject class

Представляет `VbaProject`.

```csharp
public class VbaProject
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Получает условные аргументы компиляции |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Получает описание проекта. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Получает идентификатор контекста справки проекта |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Получает имя файла справки |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Получает коллекцию [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Получает имя проекта |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Получает коллекцию [`VbaReferenceCollection`](../vbareferencecollection/) |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


