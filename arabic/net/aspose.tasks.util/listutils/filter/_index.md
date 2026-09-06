---
title: "ListUtils.Filter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ListUtils. تصفية عناصر القائمة وفقًا للشرط المحدد"
type: docs
weight: 20
url: /ar/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

تصفية عناصر القائمة وفق الشرط المحدد.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| معامل | الوصف |
| --- | --- |
| T | نوع الكائن لتطبيق الفلتر عليه. |
| قائمة | قائمة للمعالجة. |
| شرط | الشرط المستخدم لتصفية القائمة المحددة. |

### قيمة الإرجاع

القائمة المصفاة.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


