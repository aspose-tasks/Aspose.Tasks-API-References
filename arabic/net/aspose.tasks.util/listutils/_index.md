---
title: "الفئة ListUtils"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Util.ListUtils. فئة مساعدة لمعالجة القوائم"
type: docs
weight: 2740
url: /ar/net/aspose.tasks.util/listutils/
---
## ListUtils class

فئة أداة لمعالجة القوائم.

```csharp
public static class ListUtils
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | تطبيق الخوارزمية على كل عنصر في القائمة بدءاً من الموضع المحدد. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | تصفية عناصر القائمة وفق الشرط المحدد. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | العثور على أول ظهور لعنصر في القائمة يحقق الشرط المحدد. |

## الأمثلة

يعرض كيفية العمل مع طريقة Find في أداة القوائم.

```csharp
public void WorkWithListUtilsFind()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> taskFilters = project.TaskFilters.ToList();

    Assert.AreEqual(3, taskFilters.Count, "Project.TaskFilters count");

    var filter = ListUtils.Find(taskFilters, new FilterByName("&All Tasks"));

    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Filter Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

public class FilterByName : ICondition<Filter>
{
    private readonly string name;

    public FilterByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// تُعيد true إذا كان الكائن المحدد يفي بالشروط.
    /// </summary>
    /// <param name=\"el\">الكائن للتحقق منه.</param>
    /// <returns>True إذا كان الكائن يفي بالشروط.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### انظر أيضًا

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


