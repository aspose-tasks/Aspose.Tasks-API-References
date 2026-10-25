---
title: "ListUtils.Filter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ListUtils 方法。按指定条件过滤列表元素"
type: docs
weight: 20
url: /zh/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

根据指定条件过滤列表元素。

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| 参数 | 描述 |
| --- | --- |
| T | 要应用过滤器的对象类型。 |
| 列表 | 要处理的列表。 |
| 条件 | 用于过滤指定列表的条件。 |

### 返回值

过滤后的列表。

## 示例

展示如何使用列表工具的 Filter 方法。

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
    /// 如果指定的对象满足条件，则返回 true。
    /// </summary>
    /// <param name=\"el\">要检查的对象。</param>
    /// <returns>如果对象满足条件，则返回 True。</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### 另见

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)


