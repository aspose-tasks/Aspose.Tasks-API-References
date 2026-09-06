---
title: "ICondition1.Check"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ICondition 方法。 如果指定对象满足条件则返回 true"
type: docs
weight: 10
url: /zh/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

如果指定的对象满足条件，则返回 true。

```csharp
public bool Check(T el)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| el | T | 要检查的对象。 |

### 返回值

如果对象满足条件，则为 True。

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)


