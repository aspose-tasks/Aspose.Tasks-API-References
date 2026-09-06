---
title: "ICondition1.Check"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ICondition. تُرجع true إذا كان الكائن المحدد يفي بالشروط"
type: docs
weight: 10
url: /ar/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

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

يوضح كيفية العمل مع طريقة Filter في قائمة الأدوات.

```csharp
public void WorkWithListUtilsFilter()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Filter(filters, new FilterByIndex(1));

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

public class FilterByIndex : ICondition<Filter>
{
    private readonly int index;

    public FilterByIndex(int index)
    {
        this.index = index;
    }

    /// <summary>
    /// تُعيد true إذا كان الكائن المحدد يفي بالشروط.
    /// </summary>
    /// <param name=\"el\">الكائن للتحقق منه.</param>
    /// <returns>True إذا كان الكائن يفي بالشروط.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### انظر أيضًا

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


