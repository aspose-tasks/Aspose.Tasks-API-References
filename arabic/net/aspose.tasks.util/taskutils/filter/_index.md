---
title: "TaskUtils.Filter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskUtils. تُنشئ شجرة جديدة من المهام التي تُستوفي الشرط."
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

يبني شجرة جديدة من المهام التي تستوفي الشرط.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| جذر | مهمة | جذر الشجرة. |
| شرط | ICondition`1 | الشرط المطبق. |

### قيمة الإرجاع

جذر شجرة جديدة.

## الأمثلة

يظهر كيفية العمل مع شرط.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // يبني شجرة جديدة من المهام التي تُستوفي الشرط 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // جمع المهام من شجرة
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // التكرار عبر قائمة بسيطة من المهام 
    // التي تكون مدتها أكبر أو مساوية ل يومين عمل
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// تُعيد true إذا كان الكائن المحدد يفي بالشروط.
    /// </summary>
    /// <param name=\"el\">الكائن للتحقق منه.</param>
    /// <returns>True إذا كان الكائن يفي بالشروط.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


