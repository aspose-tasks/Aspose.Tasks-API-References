---
title: "Интерфейс IVbaModule"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Интерфейс Aspose.Tasks.IVbaModule. Представляет модуль с кодом VBA"
type: docs
weight: 880
url: /ru/net/aspose.tasks/ivbamodule/
---
## IVbaModule interface

Представляет модуль с кодом VBA.

```csharp
public interface IVbaModule
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Attributes](../../aspose.tasks/ivbamodule/attributes/) { get; } | Получает коллекцию [`VbaModuleAttributeCollection`](../vbamoduleattributecollection/) |
| [Name](../../aspose.tasks/ivbamodule/name/) { get; } | Получает имя модуля VBA |
| [SourceCode](../../aspose.tasks/ivbamodule/sourcecode/) { get; } | Получает исходный код VBA-модуля |

## Примеры

Показывает, как читать модули проекта VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


