---
title: "TaskUtils.Find"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskUtils. تبحث عن مهمة تلبي الشرط في شجرة من المهام"
type: docs
weight: 30
url: /ar/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

يجد مهمة تستوفي الشرط في شجرة المهام.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| جذر | مهمة | جذر الشجرة. |
| شرط | ICondition`1 | الشرط المطبق. |

### قيمة الإرجاع

المهمة إذا تم العثور على المهمة، وإلا null.

## الأمثلة

يعرض كيفية استخدام <see cref="Aspose.Tasks.Util.TaskUtils.Find" /> الطريقة.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // يبني شجرة جديدة من المهام التي تُستوفي الشرط 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// تُعيد true إذا كان الكائن المحدد يفي بالشروط.
    /// </summary>
    /// <param name=\"el\">الكائن للتحقق منه.</param>
    /// <returns>True إذا كان الكائن يفي بالشروط.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


