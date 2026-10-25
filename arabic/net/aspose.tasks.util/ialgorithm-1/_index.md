---
title: "الواجهة IAlgorithmT"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "واجهة Aspose.Tasks.Util.IAlgorithm1T. تمثّل خوارزمية يمكن تطبيقها على قائمة من الكائنات T"
type: docs
weight: 2710
url: /ar/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

يمثل خوارزمية يمكن تطبيقها على قائمة من الكائنات *T*.

```csharp
public interface IAlgorithm<in T>
```

| معامل | الوصف |
| --- | --- |
| T | نوع الكائن لتطبيق واجهة الطريقة عليه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | يعالج كائنًا في القائمة. يُستدعى بعد [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | يُستدعى بعد معالجة كائن. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | يُستدعى قبل معالجة كائن. |

## الأمثلة

يظهر كيفية العمل مع طريقة Apply في قائمة الأدوات.

```csharp
public void WorkWithListUtilsApply()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Apply(filters, new RenameAlgorithm(), 0);

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

private class RenameAlgorithm : IAlgorithm<Filter>
{
    private int current;

    public RenameAlgorithm()
    {
        this.current = 0;
    }

    public void PreAlg(Filter el, int index)
    {
        this.current++;
    }

    public void Alg(Filter el, int index)
    {
        el.Name = el.Name + " " + this.current;
    }

    public void PostAlg(Filter el, int index)
    {
    }
}
```

### انظر أيضًا

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


