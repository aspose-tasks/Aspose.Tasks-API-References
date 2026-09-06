---
title: "AndAllCondition1.AndAllCondition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ AndAllCondition. يهيئ نسخة جديدة من فئة AndAllCondition"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

يهيئ نسخة جديدة من الفئة [`AndAllCondition`](../).

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الشروط | List`1 | قائمة الشروط. |

## الأمثلة

يوضح كيفية استخدام شرط &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt;.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // جمع جميع مهام المشروع
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // إنشاء شرط تصفية يقوم بتصفية المهام غير الفارغة
                             new NotNullCondition(),

                             // إنشاء شرط تصفية يقوم بتصفية المهام الملخصة
                             new SummaryCondition()
                         };

    // وادمجهم بتطبيق شرط <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // تطبيق الشرط على المهام المجمعة
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // العمل مع خصائص أخرى...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### انظر أيضًا

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


