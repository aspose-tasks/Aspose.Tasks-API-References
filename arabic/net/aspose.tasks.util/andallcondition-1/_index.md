---
title: "الفئة AndAllConditionT"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Util.AndAllCondition1T. تُطبق العملية المنطقية AND على جميع الشروط. على سبيل المثال cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /ar/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

يطبق العملية المنطقية AND على جميع الشروط. على سبيل المثال: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| معامل | الوصف |
| --- | --- |
| T | نوع الكائن لتطبيق واجهة الطريقة عليه. |

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | يُنشئ مثلاً جديداً من الفئة `AndAllCondition`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | يرجع true إذا كان الكائن المحدد يحقق الشروط. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


