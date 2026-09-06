---
title: "ListUtils.Apply"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ListUtils. تطبيق الخوارزمية على كل عنصر في القائمة بدءًا من الموضع المحدد"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

تطبيق الخوارزمية على كل عنصر في القائمة بدءاً من الموضع المحدد.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| معامل | الوصف |
| --- | --- |
| T | نوع الكائن لتطبيق الخوارزمية عليه. |
| قائمة | قائمة للمعالجة. |
| خوارزمية | الخوارزمية المطبقة. |
| startIndex | موضع العنصر الأول. |

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

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


