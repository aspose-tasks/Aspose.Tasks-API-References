---
title: "الفئة NotT"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Util.Not1T. يطبق NOT المنطقي على الشرط المحدد"
type: docs
weight: 2750
url: /ar/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

يطبق العملية المنطقية NOT على الشرط المحدد.

```csharp
public class Not<T> : ICondition<T>
```

| معامل | الوصف |
| --- | --- |
| T | نوع الكائن لتطبيق واجهة الطريقة عليه. |

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | يُنشئ مثيلًا جديدًا للفئة `Not`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | يرجع true إذا كان الكائن المحدد يحقق الشرط. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


