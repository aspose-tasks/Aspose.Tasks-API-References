---
title: "Not1.Not"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ Not. يهيئ نسخة جديدة من الفئة Not."
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/not-1/not/
---
## Not&lt;T&gt; constructor

يهيئ نسخة جديدة من الفئة [`Not`](../).

```csharp
public Not(ICondition<T> condition)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| شرط | ICondition`1 | الشرط المحدد. |

## الأمثلة

يوضح كيفية استخدام شرط &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // جمع جميع مهام المشروع
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // إنشاء شرط تصفية
    var filter = new NullCondition();

    // وعكسه بتطبيق شرط <see cref=\"Aspose.Tasks.Util.Not`1\" />
    var condition = new Not<Task>(filter);

    // تطبيق الشرط على المهام المجمعة
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### انظر أيضًا

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


