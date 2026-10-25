---
title: "Task.ToString"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تُرجع تمثيلًا نصيًا قصيرًا لمهمة. التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير."
type: docs
weight: 1420
url: /ar/net/aspose.tasks/task/tostring/
---
## Task.ToString method

يرجع تمثيلًا نصيًا قصيرًا لمهمة. التفاصيل الدقيقة للتمثيل غير محددة وقد تتغير.

```csharp
public override string ToString()
```

### قيمة الإرجاع

نص قصير يمثل كائن المهمة.

## الأمثلة

يظهر كيفية فرز المهام حسب الاسم.

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


