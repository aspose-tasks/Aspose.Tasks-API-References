---
title: "Tsk.Resume"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. التاريخ الذي من المقرر أن تستأنف فيه الجزء المتبقي من المهمة بعد إدخال أي تقدم"
type: docs
weight: 1000
url: /ar/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

التاريخ الذي من المقرر أن تستأنف فيه الجزء المتبقي من المهمة بعد بدء أي تقدم.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
```

## الأمثلة

يوضح كيفية قراءة تواريخ إيقاف/استئناف المهمة.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحقق من تواريخ الإيقاف والاستئناف لجميع المهام.
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


