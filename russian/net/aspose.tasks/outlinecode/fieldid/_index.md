---
title: "OutlineCode.FieldId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство OutlineCode. Получает или задает числовое значение пользовательского поля Id проекта"
type: docs
weight: 20
url: /ru/net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

Получает или задает числовое значение пользовательского поля Id проекта.

```csharp
public string FieldId { get; set; }
```

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

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


