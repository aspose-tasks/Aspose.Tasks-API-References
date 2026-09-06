---
title: "IAlgorithm1.PostAlg"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة IAlgorithm. تُستدعى بعد معالجة كائن."
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/ialgorithm-1/postalg/
---
## IAlgorithm&lt;T&gt;.PostAlg method

يُستدعى بعد معالجة كائن.

```csharp
public void PostAlg(T el, int index)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| el | T | الكائن المعالج. |
| الفهرس | Int32 | فهرس الكائن. |

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

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)


