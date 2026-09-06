---
title: "OutlineCode.ValueId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineCode. تحصل أو تعين المعرف Id في قائمة القيم المرتبط بالتعريف في مجموعة كود المخطط"
type: docs
weight: 40
url: /ar/net/aspose.tasks/outlinecode/valueid/
---
## OutlineCode.ValueId property

يحصل أو يعيّن Id في قائمة القيم المرتبط بالتعريف في مجموعة كود المخطط.

```csharp
public int ValueId { get; set; }
```

## الأمثلة

يوضح كيفية قراءة أكواد المخطط التفصيلي للمهمة.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// قراءة أكواد المخطط التفصيلي
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

### انظر أيضًا

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


