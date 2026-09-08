---
title: "Класс OutlineCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OutlineCode. Представляет значение кода структуры"
type: docs
weight: 1150
url: /ru/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Представляет значение кода структуры.

```csharp
public class OutlineCode
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Инициализирует новый экземпляр класса `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Инициализирует новый экземпляр класса `OutlineCode`, используя указанный Outline Code и одно из его значений. |

## Свойства

| Имя | Описание |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Получает или задает числовое значение пользовательского поля Id проекта. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Получает или задает GUID значения в списке значений. ValueGuid соответствует FieldGuid в списке значений. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Получает или задает Id в списке значений, связанный с определением в коллекции outline code. |

## Примечания

Необходимо два элемента данных — указатель на таблицу outline code, определяемую FieldId, и значение, указанное либо через ValueId, либо через указатель ValueGuid в списке значений.

## Примеры

Показывает, как читать коды структуры задачи.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// читать коды структуры
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


