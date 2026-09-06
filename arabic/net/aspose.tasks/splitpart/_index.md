---
title: "الفئة SplitPart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.SplitPart. تمثل جزءًا من مهمة. الـ SplitPart هو عضو في مجموعة SplitParts الخاصة بالمهام."
type: docs
weight: 2290
url: /ar/net/aspose.tasks/splitpart/
---
## SplitPart class

يمثل جزءًا من المهمة. الـ SplitPart هو عضو في مجموعة SplitParts الخاصة بالمهمة.

```csharp
public class SplitPart
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | يحصل على تاريخ الانتهاء لـ SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | يحصل على تاريخ البدء لـ SplitPart. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | يقارن جزأين مقسومين. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | يرجع قيمة رمز تجزئة (hash code) للنسخة من الفئة `SplitPart`. |

## الأمثلة

يوضح كيفية العمل مع أجزاء مقسومة من مهمة مقسمة.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// يجب توليد بيانات تخصيص الموارد الزمنية أولاً
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// قسّم المهمة.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// التكرار على الأجزاء المقسمة
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


