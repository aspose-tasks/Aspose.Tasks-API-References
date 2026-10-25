---
title: "Tsk.ActualOvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التكاليف المتكبدة للعمل الإضافي الذي تم إنجازه بالفعل على المهام بواسطة الموارد المعينة"
type: docs
weight: 50
url: /ar/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

التكاليف المتكبدة للعمل الإضافي الذي تم إنجازه بالفعل على المهام بواسطة الموارد المعينة.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


