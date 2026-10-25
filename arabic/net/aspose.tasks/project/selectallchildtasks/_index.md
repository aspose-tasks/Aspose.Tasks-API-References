---
title: "Project.SelectAllChildTasks"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تجمع بشكل متكرر جميع المهام الفرعية للمهمة الجذرية"
type: docs
weight: 1230
url: /ar/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

يجمع بشكل متكرر جميع المهام الفرعية للمهمة الجذرية.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### قيمة الإرجاع

مجموعة المهام.

## الأمثلة

يظهر كيفية إعادة ترقيم رموز WBS للمهام المحددة.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// الإخراج: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// الإخراج: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### انظر أيضًا

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


