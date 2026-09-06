---
title: "OutlineCode.FieldId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineCode. تحصل أو تعين القيمة العددية لحقل المشروع المخصص Id"
type: docs
weight: 20
url: /ar/net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

يحصل أو يعيّن القيمة العددية لحقل Id المخصص للمشروع.

```csharp
public string FieldId { get; set; }
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


