---
title: "And1.And"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ And. يهيئ مثيلاً جديداً من الفئة And"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

يهيئ مثيلاً جديداً من الفئة [`And`](../).

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| cond1 | ICondition`1 | الشرط الأول. |
| cond2 | ICondition`1 | الشرط الثاني. |

## الأمثلة

يوضح كيفية استخدام شرط &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // جمع جميع مهام المشروع
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // إنشاء شرط تصفية يقوم بتصفية المهام الملخصة
    var condition1 = new SummaryCondition();

    // إنشاء شرط تصفية يقوم بتصفية المهام غير الفارغة
    var condition2 = new NotNullCondition();

    // وضمها بتطبيق شرط <see cref=\"Aspose.Tasks.Util.And`1\" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // تطبيق الشرط على المهام المجمعة
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


