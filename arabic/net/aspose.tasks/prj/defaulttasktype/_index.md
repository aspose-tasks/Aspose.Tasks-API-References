---
title: "Prj.DefaultTaskType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. النوع الافتراضي للمهام الجديدة"
type: docs
weight: 290
url: /ar/net/aspose.tasks/prj/defaulttasktype/
---
## Prj.DefaultTaskType field

نوع المهام الجديدة الافتراضي.

```csharp
public static readonly Key<TaskType, PrjKey> DefaultTaskType;
```

## الأمثلة

يظهر كيفية قراءة الخصائص الافتراضية للمشروع.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// تعيين الخصائص الافتراضية
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// عرض الخصائص الافتراضية
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


