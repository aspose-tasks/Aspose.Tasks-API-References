---
title: "OutlineCode.ValueGuid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية OutlineCode. تحصل أو تعين GUID للقيمة في قائمة القيم. يتطابق ValueGuid مع FieldGuid في قائمة القيم"
type: docs
weight: 30
url: /ar/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

يحصل أو يعيّن GUID للقيمة في قائمة القيم. يتطابق ValueGuid مع FieldGuid في قائمة القيم.

```csharp
public string ValueGuid { get; set; }
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


