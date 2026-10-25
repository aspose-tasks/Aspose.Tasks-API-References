---
title: "AndAllCondition1.Check"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة AndAllCondition. تُرجع true إذا كان الكائن المحدد يفي بالشروط"
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/andallcondition-1/check/
---
## AndAllCondition&lt;T&gt;.Check method

يرجع true إذا كان الكائن المحدد يحقق الشروط.

```csharp
public bool Check(T el)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | T | الكائن للتحقق منه. |

### قيمة الإرجاع

صحيح إذا كان الكائن يفي بالشروط.

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

* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


