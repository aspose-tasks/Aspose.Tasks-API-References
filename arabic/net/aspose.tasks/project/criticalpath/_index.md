---
title: "Project.CriticalPath"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على مجموعة تحتوي على قائمة بالمهام الحرجة التي تشكل المسار الحرج لهذا المشروع. هذه عملية On حيث n هو عدد المهام في المشروع"
type: docs
weight: 180
url: /ar/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

يحصل على مجموعة تحتوي على قائمة بالمهام الحرجة التي تشكل المسار الحرج لهذا المشروع. هذه عملية O(n)، حيث n هو عدد المهام في المشروع.

```csharp
public TaskCollection CriticalPath { get; }
```

### قيمة الإرجاع

مجموعة تمثل قائمة بجميع المهام الحرجة.

## الأمثلة

يظهر كيفية حساب المسار الحرج للمشروع.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// اعرض المسار الحرج الآن
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### انظر أيضًا

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


