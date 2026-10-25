---
title: "SplitPart.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة SplitPart. تُرجع قيمة رمز تجزئة (hash code) لنسخة من فئة SplitPart."
type: docs
weight: 40
url: /ar/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

تُرجع قيمة رمز تجزئة لنسخة فئة [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يظهر كيفية الحصول على رمز تجزئة لجزء من الانقسام.

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

// يتم التحقق من مساواة أجزاء الانقسام بالنسبة للبداية والنهاية وفهرس أجزاء الانقسام.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// رمز التجزئة لجزء من الانقسام بناءً على البداية والنهاية وفهرس الجزء.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### انظر أيضًا

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


