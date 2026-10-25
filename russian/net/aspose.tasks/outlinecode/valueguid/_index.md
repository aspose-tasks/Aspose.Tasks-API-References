---
title: "OutlineCode.ValueGuid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство OutlineCode. Получает или задает GUID значения в списке значений. ValueGuid соответствует FieldGuid в списке значений"
type: docs
weight: 30
url: /ru/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Получает или задает GUID значения в списке значений. ValueGuid соответствует FieldGuid в списке значений.

```csharp
public string ValueGuid { get; set; }
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


