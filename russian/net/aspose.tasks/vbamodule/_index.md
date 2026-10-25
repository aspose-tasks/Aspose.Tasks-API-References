---
title: "Класс VbaModule"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.VbaModule. Представляет модуль VBA"
type: docs
weight: 2810
url: /ru/net/aspose.tasks/vbamodule/
---
## VbaModule class

Представляет модуль VBA.

```csharp
public sealed class VbaModule
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Получает коллекцию атрибутов модуля. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Получает имя модуля VBA |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Получает или задает исходный код модуля VBA |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Получает тип модуля. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Создает экземпляр `VbaModule` с типом VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Создает экземпляр `VbaModule` с типом VbaModuleType.ProceduralModule. |

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


