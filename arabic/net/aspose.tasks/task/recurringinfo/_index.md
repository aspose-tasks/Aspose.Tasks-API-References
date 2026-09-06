---
title: "Task.RecurringInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. تحصل على نسخة من فئة RecurringTaskInfo للمهمة التي هي مهمة متكررة إذا لم تكن المهمة متكررة فترجع null. المعلومات عن نسخة فئة RecurringTaskInfo موجودة فقط في صيغة ملف mpp."
type: docs
weight: 1030
url: /ar/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

تحصل على نسخة من فئة [`RecurringTaskInfo`](../../recurringtaskinfo/) للمهمة التي هي مهمة متكررة؛ إذا لم تكن المهمة متكررة فترجع null؛ المعلومات عن نسخة فئة [`RecurringTaskInfo`](../../recurringtaskinfo/) موجودة فقط في صيغة ملف mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## الأمثلة

يعرض كيفية قراءة معلومات التكرار للمهمة.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### انظر أيضًا

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


