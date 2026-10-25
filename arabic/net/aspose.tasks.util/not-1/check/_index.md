---
title: "Not1.Check"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Not. تُعيد true إذا كان الكائن المحدد يفي بالشرط."
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

يرجع true إذا كان الكائن المحدد يحقق الشرط.

```csharp
public bool Check(T el)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | T | الكائن للتحقق منه. |

### قيمة الإرجاع

صحيح إذا كان الكائن يفي بالشرط.

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

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


