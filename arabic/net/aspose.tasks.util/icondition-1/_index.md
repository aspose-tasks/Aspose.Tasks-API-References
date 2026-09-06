---
title: "الواجهة IConditionT"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "واجهة Aspose.Tasks.Util.ICondition1T. تمثّل شرطاً يمكن استخدامه بواسطة الفلاتر أو طرق البحث"
type: docs
weight: 2720
url: /ar/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

يمثل شرطًا يمكن استخدامه بواسطة الفلاتر أو طرق البحث.

```csharp
public interface ICondition<in T>
```

| معامل | الوصف |
| --- | --- |
| T | نوع الكائن لتطبيق واجهة الطريقة عليه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | يرجع true إذا كان الكائن المحدد يحقق الشروط. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


