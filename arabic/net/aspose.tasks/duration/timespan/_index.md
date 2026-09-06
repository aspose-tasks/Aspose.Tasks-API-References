---
title: "Duration.TimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Duration. تحصل على نسخة TimeSpan من كائن Duration هذا. نسخة TimeSpan من كائن Duration هذا"
type: docs
weight: 40
url: /ar/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

يحصل على نسخة `TimeSpan` من كائن Duration هذا. نسخة TimeSpan من كائن Duration هذا.

```csharp
public TimeSpan TimeSpan { get; }
```

## الأمثلة

يوضح كيفية تحويل مدة إلى فترة زمنية.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// احصل على مدة المهمة
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### انظر أيضًا

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


